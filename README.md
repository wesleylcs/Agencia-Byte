# Byte Ag — Site Institucional

Site institucional da **Byte Ag**, agência de marketing digital e tecnologia. O projeto é um site estático (HTML, CSS e JavaScript puro), sem build nem dependências de backend.

🌐 **No momento, o site está visível em:** [https://wesleylcs.github.io/Agencia-Byte/](https://wesleylcs.github.io/Agencia-Byte/)

> O domínio original (byte-ag.com.br) não está mais ativo, pois o projeto não teve continuidade. O site está hospedado gratuitamente no GitHub Pages, por isso algumas referências ao domínio antigo (canonical, sitemap, robots.txt) ainda aparecem nos arquivos.

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
├── .htaccess             # Regras para Apache (ignorado no GitHub Pages)
├── robots.txt
└── sitemap.xml
```

## Recursos

- Layout responsivo
- Otimização de performance: CSS crítico, lazy-load de imagens, fontes locais e hero com gradiente (sem imagem pesada)
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

> As regras do `.htaccess` só funcionam em servidores Apache. No GitHub Pages elas são ignoradas.

## Configuração antes de usar como base

Se você for reutilizar este projeto, troque:

- ID do Google Tag Manager (`GTM-...`) nos arquivos HTML
- E-mail de destino do formulário (FormSubmit)
- Número do WhatsApp (links `wa.me`)
- Domínio em `.htaccess`, `sitemap.xml` e `robots.txt`

## Licença

Todos os direitos reservados © Byte Ag. Textos, imagens e identidade visual não podem ser reutilizados sem autorização.
