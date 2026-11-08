# Impostor & Inocente Online 👻

Jogo multiplayer de navegador com salas (*parties*), papéis de impostor e inocente e modo fantasma.

## Arquivos

- `index.html`: site do jogo, com interface, JavaScript e efeitos sonoros.
- `README.md`: documentação do projeto; não é necessário para executar o jogo.
- `impostor_inocente_completo_supabase.sql`: script de configuração do banco de dados (executado no Supabase, não no GitHub Pages).

## Publicar no GitHub Pages

1. Crie um repositório público no GitHub.
2. Envie `index.html` e `README.md` para a raiz do repositório.
3. Vá a **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**, branch `main` e pasta `/ (root)`; salve.
5. Aguarde a publicação e acesse o endereço indicado na página de configurações.

## Configurar o Supabase

1. Crie um projeto em [Supabase](https://supabase.com/dashboard).
2. Execute o script SQL no **SQL Editor** (idealmente em um projeto novo).
3. Ative **Authentication → Providers → Anonymous Sign-ins**.
4. Configure a URL do projeto e a **publishable key** no jogo, se necessário. Nunca use uma `secret key` ou `service_role` no HTML.
5. Abra o site publicado em dois navegadores/dispositivos diferentes para testar criação e entrada em parties.

## Mecânicas planejadas/implementadas na versão de teste

- Nome de jogador e criação/entrada em party.
- Anfitrião inicia a partida; papéis são sorteados.
- Impostor pode selecionar uma vítima para Kill.
- Jogador eliminado continua como fantasma e pode fazer tarefas.
- Sabotagem e report enviam alertas aos participantes.
- Efeitos sonoros para Kill, Task, Sabotar e Reportar.

**Atenção:** o multiplayer depende do Supabase e ainda precisa de testes reais entre dispositivos. O README não instala o banco nem ativa o multiplayer sozinho. Não há ainda votação ou condição completa de vitória.
