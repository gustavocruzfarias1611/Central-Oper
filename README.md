# Central Cruz & Farias

Plataforma corporativa completa para centralizar sistemas, treinamentos, chamados, cadastros, processos, documentos, indicadores e assistência por IA.

## Recursos incluídos

- Dashboard executivo com indicadores e gráficos;
- Ecossistema de sistemas: Sienge, Sankhya, WMS Senior, Prevision, Mobuss e SoftExpert;
- Universidade corporativa e trilhas de treinamento;
- Central de chamados com filtros, prioridades e SLA;
- Central de cadastros de produtos, parceiros, usuários e estruturas operacionais;
- Processos e fluxos visualizados etapa por etapa;
- Base de conhecimento com pesquisa de documentos;
- Assistente corporativa ÍRIS;
- Busca global com atalho `Ctrl + K`;
- Notificações laterais;
- Configurações de perfil, aparência, integrações e segurança;
- Página detalhada com as características da plataforma;
- Layout responsivo para celular, tablet, notebook e desktop.

## Tecnologias

- React 19;
- Next.js 16;
- TypeScript;
- CSS responsivo;
- Vinext/Vite para publicação em Cloudflare Workers.

## Rodar localmente

Requisitos: Node.js 22.13 ou superior e npm.

```bash
npm install
npm run dev
```

Abra o endereço mostrado no terminal, normalmente `http://localhost:3000`.

## Gerar a versão de produção

```bash
npm run build
npm run start
```

## Publicar

### OpenAI Sites

O projeto já possui a configuração necessária na pasta `.openai`. Abra o projeto no Sites e publique uma nova versão.

### GitHub

1. Crie um repositório vazio no GitHub;
2. Envie todos os arquivos deste projeto;
3. Mantenha `package-lock.json` junto com `package.json`;
4. Configure o serviço de hospedagem para usar `npm run build`.

### Cloudflare

O projeto utiliza Worker compatível com Vinext. Faça a implantação usando o fluxo de Cloudflare Workers adotado pela sua conta.

## Estrutura principal

- `app/page.tsx`: páginas, conteúdos e interações da central;
- `app/globals.css`: identidade visual e responsividade;
- `app/layout.tsx`: metadados e estrutura global;
- `public/`: arquivos públicos;
- `worker/`: entrada da aplicação em produção;
- `package.json`: dependências e comandos do projeto.

## Personalização

Os textos, sistemas, indicadores, usuários, cursos e processos demonstrativos ficam em `app/page.tsx`. Cores, espaçamentos, componentes e regras responsivas ficam em `app/globals.css`.

---

Desenvolvido para a Cruz & Farias Consultoria.
