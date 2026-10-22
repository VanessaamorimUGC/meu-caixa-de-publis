# Meu Caixa de Publis

Aplicativo web responsivo para registrar campanhas, valores, datas, entregas e status de pagamento.

## Arquivos
- `index.html`: aplicativo completo.
- `manifest.webmanifest`, `sw.js` e ícones: instalação como PWA e cache offline.

## Dados e recuperação
Os registros são guardados no armazenamento local (`localStorage`) do navegador/dispositivo. Não há sincronização automática em nuvem. Limpar os dados do navegador, usar navegação privada ou trocar de aparelho pode apagar/deixar os registros inacessíveis. Use **Exportar / backup → Backup completo (JSON)** com frequência e guarde uma cópia no iCloud Drive, Google Drive ou Arquivos. Para recuperar, abra o app, escolha **Exportar / backup**, selecione o JSON e toque em **Restaurar**. CSV é para planilhas e não é o formato de restauração.

## Publicar grátis pelo celular com GitHub Pages
1. No Safari, acesse https://github.com e crie uma conta ou entre.
2. Toque no `+` → **New repository**. Nome sugerido: `meu-caixa-de-publis`. Marque **Public** e crie o repositório.
3. Na página do repositório, toque em **Add file** → **Upload files**.
4. Envie TODOS os arquivos desta pasta, mantendo os nomes e a estrutura: `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`. Se estiver no celular, primeiro descompacte o ZIP no app Arquivos e selecione os arquivos.
5. Toque em **Commit changes**.
6. No repositório, abra **Settings** → **Pages**. Em **Build and deployment**, selecione **Deploy from a branch**; branch `main`, pasta `/(root)` e **Save**.
7. Aguarde o GitHub publicar. A URL normalmente será `https://SEU-USUARIO.github.io/meu-caixa-de-publis/`. Substitua `SEU-USUARIO` pelo seu usuário real. Não considere publicado até abrir esse endereço no Safari e ver a tela inicial do app.
8. Se der 404, confira se `index.html` está na raiz e se Pages está apontando para `main` e `/(root)`. Aguarde alguns minutos e tente novamente.

## Adicionar à tela inicial do iPhone
1. Abra a URL publicada no **Safari** (não dentro do navegador do Instagram).
2. Toque no botão **Compartilhar** (quadrado com seta para cima).
3. Role a lista e toque em **Adicionar à Tela de Início**. Se aparecer, habilite **Abrir como app**.
4. Toque em **Adicionar**. O ícone “Caixa de Publis” aparecerá na tela inicial.

## Importante sobre confiabilidade
A publicação torna o app acessível pela internet, mas não transforma o armazenamento local em nuvem. Os dados ficam neste navegador. Para sincronizar entre iPhone e outros dispositivos, seria necessário configurar uma base de dados e autenticação (por exemplo, Supabase); este projeto não está conectado a esse serviço. Faça backup regular, especialmente antes de limpar o Safari ou trocar de aparelho.
