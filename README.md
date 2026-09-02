# Eufránio & Creuma — Wedding Website

Site estático em HTML + CSS + JavaScript puro, construído a partir do design fornecido.

## Estrutura

- `index.html` — estrutura completa da página
- `css/style.css` — design, responsividade e animações
- `js/script.js` — countdown, reveal animations e copiar dados bancários
- `assets/floral-corner.png` — elemento floral usado nos quatro cantos do hero

## Como adicionar as fotografias

Os espaços das fotografias foram deixados intencionalmente vazios, sem mensagens auxiliares.

No `index.html`, procure por:
- `.hero-photo`
- `.story-photo`

Pode colocar uma imagem dentro de cada `.photo-slot`, por exemplo:

```html
<div class="hero-photo photo-slot">
  <img src="assets/foto-1.jpg" alt="Eufránio e Creuma">
</div>
```

Depois, se quiser que a fotografia preencha o espaço:

```css
.photo-slot img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

## Countdown

A data está configurada em `js/script.js`:

`2026-09-27T19:00:00+01:00`

O efeito dos números sobe como uma folha de papel quando cada unidade muda.

## Dados para contribuição

Os dados já estão incluídos:

- Beneficiário: EUFRÁNIO LUKENY MANUEL DIOGO
- IBAN: AO06 0006 0000 0521 9535 302 77
- Multicaixa Express: 922 873 628
- Kwik: mesmo IBAN e beneficiário

Cada dado possui botão para copiar.

## Executar

Pode abrir `index.html` diretamente no navegador ou usar qualquer servidor estático.

Exemplo:

```bash
python3 -m http.server 8080
```

Depois abrir `http://localhost:8080`.
