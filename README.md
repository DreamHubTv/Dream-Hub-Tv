# Dream-Hub-Tv
import { Button } from "@/components/ui/button"; import { Card, CardContent } from "@/components/ui/card"; import { PhoneCall, PlayCircle, Tv } from "lucide-react";

export default function DreamHubTV() { return ( <div className="bg-[#0B0F25] text-white min-h-screen font-sans"> <header className="p-6 text-center border-b border-white/10"> <h1 className="text-3xl md:text-5xl font-bold text-white"> Dream Hub Entertainment </h1> <p className="text-blue-300 mt-2 text-lg"> Canais, filmes e séries na palma da sua mão </p> </header>

<section className="p-6 md:p-12 grid md:grid-cols-2 gap-8 items-center">
    <div>
      <h2 className="text-2xl md:text-3xl font-semibold mb-4">
        Sua nova experiência de entretenimento
      </h2>
      <ul className="space-y-2 text-blue-100 text-base">
        <li className="flex items-center gap-2">
          <Tv className="w-5 h-5 text-blue-500" /> Mais de 2.500 canais ao vivo
        </li>
        <li className="flex items-center gap-2">
          <PlayCircle className="w-5 h-5 text-blue-500" /> 13.000+ filmes e 4.000+ séries
        </li>
        <li className="flex items-center gap-2">
          <PlayCircle className="w-5 h-5 text-blue-500" /> Qualidade HD e 4K
        </li>
        <li className="flex items-center gap-2">
          <PlayCircle className="w-5 h-5 text-blue-500" /> Compatível com TV, celular, computador e mais
        </li>
      </ul>
      <Button className="mt-6 bg-blue-600 hover:bg-blue-700 text-white text-lg px-6 py-3 rounded-2xl shadow-xl" asChild>
        <a href="https://wa.me/5514996353155" target="_blank">
          Teste Gratuito via WhatsApp
        </a>
      </Button>
    </div>
    <img
      src="https://images.unsplash.com/photo-1600965962473-3b5c2114d37b"
      alt="TV" className="rounded-2xl shadow-xl"
    />
  </section>

  <section className="p-6 md:p-12 bg-[#10172A]">
    <h2 className="text-2xl md:text-3xl font-semibold text-center mb-8">
      Planos
    </h2>
    <div className="grid md:grid-cols-2 gap-6 max-w-4xl mx-auto">
      <Card className="bg-[#19223B] text-white rounded-2xl shadow-xl">
        <CardContent className="p-6">
          <h3 className="text-xl font-semibold mb-2">Plano Mensal</h3>
          <p className="text-blue-300 mb-4">R$ 29,90/mês</p>
          <p className="text-sm text-blue-100 mb-4">
            Pagamento via PIX ou boleto bancário.
          </p>
          <Button className="w-full bg-blue-600 hover:bg-blue-700" asChild>
            <a href="https://wa.me/5514996353155" target="_blank">
              Assinar Mensal
            </a>
          </Button>
        </CardContent>
      </Card>

      <Card className="bg-[#19223B] text-white rounded-2xl shadow-xl">
        <CardContent className="p-6">
          <h3 className="text-xl font-semibold mb-2">Plano Anual</h3>
          <p className="text-blue-300 mb-4">R$ 238,80/ano</p>
          <p className="text-sm text-blue-100 mb-4">
            Pagamento via PIX, boleto ou em até 12x no cartão (com taxa de parcelamento).
          </p>
          <Button className="w-full bg-blue-600 hover:bg-blue-700" asChild>
            <a href="https://wa.me/5514996353155" target="_blank">
              Assinar Anual
            </a>
          </Button>
        </CardContent>
      </Card>
    </div>
  </section>

  <footer className="p-6 text-center text-sm text-blue-200 bg-[#0B0F25] border-t border-white/10">
    Dream Hub Entertainment © {new Date().getFullYear()} – Todos os direitos reservados.
  </footer>
</div>

); }

