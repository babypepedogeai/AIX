// BabyPepeDogeAI Website

import React from "react";
import Image from "next/image";
import { Button } from "@/components/ui/button";
import { Rocket, MessageCircle, Infinity, Copy } from "lucide-react";

export default function HomePage() {
  return (
    <div className="min-h-screen bg-black text-white font-sans">
      {/* Hero Section */}
      <section className="text-center py-24 px-4 bg-gradient-to-br from-black via-gray-900 to-black relative">
        <Image
          src="/aixxx22.png"
          alt="BabyPepeDogeAI Banner"
          width={600}
          height={300}
          className="mx-auto rounded-2xl shadow-xl"
        />
        <h1 className="text-6xl font-bold mt-6">
          BabyPepe<span className="text-pink-500">Doge</span>AI <span className="text-yellow-400">∞</span>
        </h1>
        <p className="text-xl text-gray-300 mt-4 max-w-2xl mx-auto">
          Memes Meet AI. Doge Drives. Pepe Commands. ∞ Powered.
        </p>
        <div className="mt-6 flex justify-center space-x-4">
          <Button className="bg-pink-600 hover:bg-pink-700 text-white text-lg">
            Buy $AIX∞
          </Button>
          <Button variant="outline" className="text-white border-white">
            View Tokenomics
          </Button>
        </div>
      </section>

      {/* Tokenomics Section */}
      <section className="py-16 px-6 text-center">
        <h2 className="text-4xl font-bold mb-6">Tokenomics</h2>
        <p className="text-lg text-gray-300 mb-4">Explore the memeconomy behind $AIX∞</p>
        <div className="flex justify-center items-center space-x-2 text-sm text-gray-400">
          <span className="bg-white text-black px-2 py-1 rounded font-mono">Contract:</span>
          <code className="bg-gray-800 px-2 py-1 rounded">BDZvYmp4pC9ssxQsERyjhqqzcx3YkK1uPAvNdaNypump</code>
          <Button variant="ghost" size="icon" className="text-white hover:text-green-400">
            <Copy className="w-4 h-4" />
          </Button>
        </div>
      </section>

      {/* Meme Gallery */}
      <section className="py-16 px-6 bg-gradient-to-br from-purple-900 to-black text-center">
        <h2 className="text-4xl font-bold mb-10">🔥 Meme Gallery</h2>
        <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 max-w-6xl mx-auto">
          <Image src="/meme1.png" alt="Meme 1" width={300} height={300} className="rounded-xl shadow-lg" />
          <Image src="/meme2.png" alt="Meme 2" width={300} height={300} className="rounded-xl shadow-lg" />
          <Image src="/meme3.png" alt="Meme 3" width={300} height={300} className="rounded-xl shadow-lg" />
        </div>
      </section>

      {/* Social Links */}
      <section className="py-16 px-6 bg-black text-center">
        <h2 className="text-4xl font-bold mb-6">Join the Memevolution 🧠</h2>
        <p className="text-lg text-gray-400 mb-6">We’re building the memeconomy with $AIX∞. Come build chaos with us.</p>
        <div className="flex flex-wrap justify-center gap-4">
          <a href="https://x.com/babypepedogeai1" target="_blank" rel="noopener">
            <Button variant="outline" className="text-white border-white">
              <Rocket className="mr-2 h-5 w-5" /> Twitter
            </Button>
          </a>
          <a href="https://t.me/BabyPepeDogeAicoin" target="_blank" rel="noopener">
            <Button variant="outline" className="text-white border-white">
              <MessageCircle className="mr-2 h-5 w-5" /> Telegram
            </Button>
          </a>
          <a href="https://pump.fun/BDZvYmp4pC9ssxQsERyjhqqzcx3YkK1uPAvNdaNypump" target="_blank" rel="noopener">
            <Button variant="outline" className="text-white border-white">
              <Infinity className="mr-2 h-5 w-5" /> Pump.fun
            </Button>
          </a>
        </div>
      </section>
    </div>
  );
}
