# Meus Afazeres (Jarvis)

Sistema pessoal de tarefas, rotinas e agenda, integrado ao Outlook (Microsoft 365).

- Empresas/áreas (R. Nunes, JF, Magi, Pessoal) → projetos/obras → rotinas, entregas, reuniões e tarefas
- Rotinas recorrentes: diária, semanal, mensal (dia fixo ou "n-ésima semana")
- Visões: Hoje, Semana, Calendário (semana/mês)
- Outlook via Microsoft Graph: lê sua agenda e as compartilhadas, cria/edita eventos com lembrete
- Dados salvos no OneDrive do usuário: `Apps/MeusAfazeres/dados.json` (cópia diária em `backups/`)

Página estática (GitHub Pages). Nenhum dado pessoal fica neste repositório.

## Configuração no Microsoft Entra
Registro de aplicativo → Autenticação → Aplicativo de página única (SPA) com a URI do site publicado.
Permissões delegadas do Microsoft Graph: `User.Read`, `Calendars.ReadWrite`, `Calendars.ReadWrite.Shared`, `Files.ReadWrite`, `offline_access`.
