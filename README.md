import { Card, CardContent } from "@/components/ui/card";
import { Badge } from "@/components/ui/badge";
import { Button } from "@/components/ui/button";
import { Mail, Phone, MapPin, Github, Linkedin } from "lucide-react";

export default function OsamaCV() {
  return (
    <div className="p-6 md:p-12 bg-slate-50 text-slate-800 font-sans">
      <div className="max-w-4xl mx-auto">
        {/* Header */}
        <div className="text-center mb-10">
          <h1 className="text-4xl font-bold text-blue-700">Osama Abu Arra</h1>
          <p className="text-lg font-medium">Software Developer</p>
        </div>

        {/* Contact */}
        <div className="grid grid-cols-1 md:grid-cols-2 gap-4 text-sm mb-10">
          <div className="flex items-center gap-2"><Phone size={16}/> +972 59-512-6144</div>
          <div className="flex items-center gap-2"><Mail size={16}/> osama54arra@gmail.com</div>
          <div className="flex items-center gap-2"><MapPin size={16}/> Aqqaba, Tubas, Palestine</div>
          <div className="flex items-center gap-2"><Github size={16}/> github.com/osama54arra</div>
          <div className="flex items-center gap-2"><Linkedin size={16}/> linkedin.com/in/osama54arra</div>
        </div>

        {/* About Me */}
        <Card className="mb-8">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold text-blue-600 mb-2">About Me</h2>
            <p>
              Motivated and detail-oriented Computer Science graduate with solid experience in full-stack development through real-world internships. Demonstrated skills in building scalable web applications using React.js, ASP.NET, and SQL Server. Strong interest in artificial intelligence, computer vision, and game development. Eager to contribute to impactful software projects while continuously learning and growing in a dynamic environment.
            </p>
          </CardContent>
        </Card>

        {/* Experience */}
        <Card className="mb-8">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold text-blue-600 mb-4">Experience</h2>
            <div className="mb-4">
              <h3 className="font-bold">Software Engineer Intern – Bilsan Business Solutions</h3>
              <p className="text-sm text-gray-600">Mar 2025 – Present</p>
              <ul className="list-disc ml-5 mt-2 space-y-1 text-sm">
                <li>Developed beginner-level full-stack web applications using Next.js, ASP.NET, and SQL Server.</li>
                <li>Contributed to scalable software architecture and backend infrastructure.</li>
                <li>Implemented AI-driven solutions in computer vision and data processing.</li>
                <li>Designed UI/UX prototypes using Figma to improve user experience.</li>
                <li>Participated in a government project for automating official car transactions.</li>
                <li>Built and trained a custom AI model tailored for internal company use.</li>
              </ul>
            </div>
            <div>
              <h3 className="font-bold">Software Developer Intern – Dimensions Information Technology</h3>
              <p className="text-sm text-gray-600">Jun 2024 – Nov 2024</p>
              <ul className="list-disc ml-5 mt-2 space-y-1 text-sm">
                <li>Gained practical experience in full-stack development with React.js and ASP.NET.</li>
                <li>Enhanced front-end functionality and performance using modern JavaScript frameworks.</li>
                <li>Worked on real-world applications with direct involvement in team-based projects.</li>
              </ul>
            </div>
          </CardContent>
        </Card>

        {/* Education & Certifications */}
        <div className="grid md:grid-cols-2 gap-6 mb-8">
          <Card>
            <CardContent className="p-6">
              <h2 className="text-2xl font-semibold text-blue-600 mb-2">Education</h2>
              <p className="font-bold">Bachelor of Computer Science</p>
              <p className="text-sm text-gray-600">Arab American University | Oct 2021 – Mar 2025</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-6">
              <h2 className="text-2xl font-semibold text-blue-600 mb-2">Certification</h2>
              <p className="font-bold">First Responder Paramedic</p>
              <p className="text-sm text-gray-600">Palestinian Red Crescent | 2022</p>
            </CardContent>
          </Card>
        </div>

        {/* Technical Skills */}
        <Card className="mb-8">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold text-blue-600 mb-2">Technical Skills</h2>
            <div className="flex flex-wrap gap-2">
              {[
                "Python", "Java", "JavaScript", "C#", "C++", "HTML", "CSS", "SCSS", "SQL",
                "React", "Bootstrap", "ASP.NET", "Next.js", "GitHub", "Figma", "jQuery",
                "NumPy", "Pandas", "SQL Server", "OOP", "Data Structures", "Algorithms",
                "AI Fundamentals", "Computer Vision", "Game Development"
              ].map(skill => (
                <Badge key={skill} variant="outline" className="text-blue-700 border-blue-300">{skill}</Badge>
              ))}
            </div>
          </CardContent>
        </Card>

        {/* Languages & References */}
        <div className="grid md:grid-cols-2 gap-6">
          <Card>
            <CardContent className="p-6">
              <h2 className="text-2xl font-semibold text-blue-600 mb-2">Languages</h2>
              <p>Arabic: Native</p>
              <p>English: Intermediate to Advanced</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-6">
              <h2 className="text-2xl font-semibold text-blue-600 mb-2">References</h2>
              <p className="font-bold">Sanad Malaysha – Faculty Lecturer, AAUP</p>
              <p>Phone: +972 59-455-8090</p>
              <p>Email: sanad.malaysha@aaup.edu</p>
            </CardContent>
          </Card>
        </div>
      </div>
    </div>
  );
}
