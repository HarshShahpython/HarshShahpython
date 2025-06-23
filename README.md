import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Linkedin } from "lucide-react";

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gray-950 text-white px-6 py-12 font-sans">
      <header className="text-center mb-12">
        <h1 className="text-4xl md:text-5xl font-bold mb-4">Hi 👋, I'm Harsh Shah</h1>
        <p className="text-xl md:text-2xl text-gray-400">
          Strategic Customer Success Manager | SaaS Expert | Cloud Enthusiast
        </p>
        <div className="flex justify-center mt-6 gap-4">
          <Button asChild variant="outline">
            <a href="mailto:haarsh.shahh@gmail.com" target="_blank">
              <Mail className="mr-2" /> Email
            </a>
          </Button>
          <Button asChild variant="outline">
            <a href="https://www.linkedin.com/in/harshashwinshah" target="_blank">
              <Linkedin className="mr-2" /> LinkedIn
            </a>
          </Button>
        </div>
      </header>

      <section className="mb-12 max-w-4xl mx-auto">
        <h2 className="text-3xl font-semibold mb-6 text-teal-400">About Me</h2>
        <p className="text-gray-300 leading-relaxed">
          I’m a Customer Success Leader and Product Management enthusiast with over 5 years of experience in SaaS and
          digital marketing. I specialize in client retention, digital strategy, product adoption, and stakeholder
          engagement. Currently upskilling in AWS Cloud and Product Lifecycle Management.
        </p>
      </section>

      <section className="mb-12 max-w-4xl mx-auto">
        <h2 className="text-3xl font-semibold mb-6 text-teal-400">Experience Highlights</h2>
        <Card className="mb-4">
          <CardContent className="p-6">
            <h3 className="text-xl font-bold">Strategic Customer Success Manager – Milestone Inc (Toronto, Canada)</h3>
            <p className="text-sm text-gray-400">Mar 2024 – Present</p>
            <ul className="list-disc list-inside text-gray-300 mt-2">
              <li>Managing enterprise franchise clients across North America</li>
              <li>Leading onboarding and campaign execution across SEO, PPC, and analytics</li>
              <li>Delivering performance reports and QBRs to C-level clients</li>
              <li>Driving retention and upsell strategies</li>
            </ul>
          </CardContent>
        </Card>

        <Card className="mb-4">
          <CardContent className="p-6">
            <h3 className="text-xl font-bold">Customer Success Manager – Milestone Internet Pvt Ltd (India)</h3>
            <p className="text-sm text-gray-400">Mar 2023 – Feb 2024</p>
            <ul className="list-disc list-inside text-gray-300 mt-2">
              <li>Managed 30+ B2B accounts with 95%+ retention</li>
              <li>Improved NPS and reduced Time-to-Value by 20%</li>
              <li>Led upsell initiatives and client onboarding programs</li>
            </ul>
          </CardContent>
        </Card>

        <Card className="mb-4">
          <CardContent className="p-6">
            <h3 className="text-xl font-bold">Product Specialist – Adit</h3>
            <p className="text-sm text-gray-400">Oct 2021 – Mar 2023</p>
            <ul className="list-disc list-inside text-gray-300 mt-2">
              <li>Launched SaaS product that scaled to $1.8M/month</li>
              <li>Led onboarding for 120+ clients</li>
              <li>Implemented client-requested features</li>
            </ul>
          </CardContent>
        </Card>
      </section>

      <section className="mb-12 max-w-4xl mx-auto">
        <h2 className="text-3xl font-semibold mb-6 text-teal-400">Certifications & Learning</h2>
        <ul className="list-disc list-inside text-gray-300">
          <li>AWS Certified Cloud Practitioner (in progress)</li>
          <li>Product Management – IBM (Coursera)</li>
          <li>Google Digital Marketing & E-Commerce (2024)</li>
          <li>Key Account Management, Totango Success Dreamer</li>
        </ul>
      </section>

      <footer className="text-center text-sm text-gray-500">
        &copy; {new Date().getFullYear()} Harsh Shah. All rights reserved.
      </footer>
    </div>
  );
}
