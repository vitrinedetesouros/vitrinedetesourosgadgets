import React from "react";

const marketplaces = [
  { name: "Amazon", link: "https://amzn.to/4fT068n" },
  { name: "Shopee", link: "https://collshp.com/vitrinedetesouros" },
  { name: "Fechadura Digital Intelbras FR 101", link: "https://mercadolivre.com/sec/1CNW2Vm" },
  { name: "Parafusadeira Furadeira The Black Tools TB-21PX", link: "https://mercadolivre.com/sec/1jRknYU" },
  { name: "Serra Mármore Makita 1300w 4.3/8", link: "https://mercadolivre.com/sec/2eFLRQk" },
  { name: "Fone de Ouvido Bluetooth Wave Buds 2 JBL", link: "https://mercadolivre.com/sec/1hFnkqL" },
];

export default function App() {
  return (
    <div className="p-6">
      <h1 className="text-2xl font-bold mb-4">Marketplace</h1>
      <div className="flex flex-col gap-2 mb-6">
        {marketplaces.map((m, i) => (
          <a
            key={i}
            href={m.link}
            target="_blank"
            rel="noopener noreferrer"
            className="bg-yellow-300 px-4 py-2 rounded-md"
          >
            Visitar {m.name}
          </a>
        ))}
      </div>
    </div>
  );
}
