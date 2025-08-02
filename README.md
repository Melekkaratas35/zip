import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Github, Linkedin } from "lucide-react";

export default function Portfolio() {
  return (
    <div className="p-6 max-w-5xl mx-auto space-y-10">
      {/* Ana Giriş */}
      <section className="text-center space-y-3">
        <h1 className="text-4xl font-bold">Melek Karataş</h1>
        <p className="text-lg text-muted-foreground">
          Biomedical Engineering Student | Research & Development Enthusiast
        </p>
        <div className="flex justify-center gap-4">
          <a href="mailto:mellek.karatas35@gmail.com">
            <Button variant="outline"><Mail className="mr-2 h-4 w-4" /> E-mail</Button>
          </a>
          <a href="https://www.linkedin.com/in/melek-karata%C5%9F-b200277mk" target="_blank">
            <Button variant="outline"><Linkedin className="mr-2 h-4 w-4" /> LinkedIn</Button>
          </a>
          <a href="https://github.com/your-github" target="_blank">
            <Button variant="outline"><Github className="mr-2 h-4 w-4" /> GitHub</Button>
          </a>
        </div>
      </section>

      {/* Hakkımda */}
      <section className="space-y-4">
        <h2 className="text-2xl font-semibold">About Me</h2>
        <p>
          I am a third-year Biomedical Engineering student at Katip Çelebi University in İzmir, Türkiye, also studying Healthcare Management via distance learning. I have hands-on experience in calibration, sterilization systems, and diagnostics, and a deep interest in neurotechnology and human-machine interaction.
        </p>
      </section>

      {/* Projeler */}
      <section className="space-y-4">
        <h2 className="text-2xl font-semibold">Projects</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-semibold">Teknofest Mentorship</h3>
              <p>Provided guidance to student teams in biomedical and healthcare-themed projects at Turkey's biggest tech festival.</p>
            </CardContent>
          </Card>

          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-semibold">Cyber Security Trainings (T3 Foundation)</h3>
              <p>Conducted Kali Linux training sessions for beginners as part of Türkiye’s national technology initiative.</p>
            </CardContent>
          </Card>

          <Card>
            <CardContent className="p-4">
              <h3 className="text-xl font-semibold">Sterilizer Assembly Internship</h3>
              <p>Interned at Kordon Tıp Ltd., gaining practical experience in device calibration, quality control, and production lines.</p>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* Eğitim */}
      <section className="space-y-4">
        <h2 className="text-2xl font-semibold">Education</h2>
        <ul className="list-disc list-inside">
          <li><strong>Katip Çelebi University</strong> – B.Sc. in Biomedical Engineering (2020–2025)</li>
          <li><strong>Anadolu University</strong> – B.A. in Healthcare Management (2022–2026)</li>
        </ul>
      </section>

      {/* Medya / Ekstralar */}
      <section className="space-y-4">
        <h2 className="text-2xl font-semibold">Media & Downloads</h2>
        <ul className="list-disc list-inside">
          <li><a href="/cv-melek-karatas-2024.pdf" className="underline text-blue-600" download>Download My CV (PDF)</a></li>
          <li><a href="/your-project-poster.png" className="underline text-blue-600" target="_blank">View Teknofest Poster</a></li>
        </ul>
      </section>
    </div>
  );
}

