# Byte Ag — Site Institucional

Site institucional da **Byte Ag** ([byte-ag.com.br](https://www.byte-ag.com.br)), agência de marketing digital e tecnologia. O projeto é um site estático (HTML, CSS e JavaScript puro), sem build nem dependências de backend, pensado para hospedagem tradicional em Apache (`public_html`).

## Serviços apresentados

- Criação de sites
- SEO para negócios
- Gestão de tráfego pago
- Gestão de redes sociais
- Google Meu Negócio
- Dashboards

## Estrutura

```
.
├── index.html            # Página inicial
├── obrigado.html         # Página de agradecimento pós-formulário
├── servicos/             # Uma página por serviço
├── css/                  # Estilos (critical, minificado, fontes, Font Awesome)
├── fonts/ e webfonts/    # Poppins, Space Grotesk e Font Awesome (hospedados localmente)
├── imgs/                 # Imagens (maioria em WebP)
├── script.js             # Menu, FAQ, depoimentos, lazy-load e envio de formulários
├── .htaccess             # HTTPS, www, redirecionamentos, cache, gzip e headers de segurança
├── robots.txt
└── sitemap.xml
```

## Recursos

- Layout responsivo
- Otimização de performance: CSS crítico, lazy-load de imagens, fontes locais, compressão e cache via `.htaccess`
- SEO: sitemap, robots.txt e redirecionamentos 301
- Formulário de contato via [FormSubmit](https://formsubmit.co)
- Botão flutuante de WhatsApp
- Google Tag Manager para métricas

## Como rodar localmente

Não há etapa de build. Abra o `index.html` no navegador ou sirva a pasta com qualquer servidor estático:

```bash
npx serve .
# ou
python -m http.server 8000
```

> As regras do `.htaccess` só funcionam em servidores Apache com `mod_rewrite`, `mod_expires`, `mod_deflate` e `mod_headers`.

## Configuração antes de usar como base

Se você for reutilizar este projeto, troque:

- ID do Google Tag Manager (`GTM-...`) nos arquivos HTML
- E-mail de destino do formulário (FormSubmit)
- Número do WhatsApp (links `wa.me`)
- Domínio em `.htaccess`, `sitemap.xml` e `robots.txt`

## Licença

Todos os direitos reservados © Byte Ag. Textos, imagens e identidade visual não podem ser reutilizados sem autorização.
