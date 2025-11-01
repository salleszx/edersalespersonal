import { Home, User, Briefcase, Target, Award, Phone } from "lucide-react";
import { NavBar } from "@/components/ui/tubelight-navbar";
import { Hero } from "@/components/Hero";
import { SplineSceneSection } from "@/components/SplineSceneSection";
import { ScrollShowcase } from "@/components/ScrollShowcase";
import { Sobre } from "@/components/Sobre";
import { Atuacao } from "@/components/Atuacao";
import { Metodo } from "@/components/Metodo";
import { Beneficios } from "@/components/Beneficios";
import { Contato } from "@/components/Contato";
import { WhatsAppButton } from "@/components/WhatsAppButton";

const navItems = [
  { name: "Início", url: "inicio", icon: Home },
  { name: "Sobre", url: "sobre", icon: User },
  { name: "Atuação", url: "atuacao", icon: Briefcase },
  { name: "Método", url: "metodo", icon: Target },
  { name: "Benefícios", url: "beneficios", icon: Award },
  { name: "Contato", url: "contato", icon: Phone },
];

const Index = () => {
  return (
    <div className="min-h-screen">
      <NavBar items={navItems} />
      <Hero />
      <SplineSceneSection />
      <ScrollShowcase />
      <Sobre />
      <Atuacao />
      <Metodo />
      <Beneficios />
      <Contato />
      <WhatsAppButton />
    </div>
  );
};

export default Index;
