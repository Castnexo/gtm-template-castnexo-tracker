# Castnexo Tracker — Tag do Google Tag Manager

Tag (Custom Template) para **Google Tag Manager Web** que instala o script de
rastreamento do **Castnexo Tracker** no site, sem precisar colar código no
HTML manualmente.

## Para que serve

O Castnexo Tracker é uma plataforma de analytics e tracking intelligence:
captura origem de tráfego, comportamento do usuário e conversões com
atribuição. Este template injeta o script do tracker e configura o workspace
diretamente pela interface do GTM.

## Pré-requisito

Uma conta no Castnexo com um workspace ativo. O **Workspace ID** é obtido na
página de Instalação do painel ([castnexo.com.br](https://castnexo.com.br)).
Sem uma conta Castnexo, o script não coleta dados.

## Configuração

| Campo | Obrigatório | Descrição |
|-------|-------------|-----------|
| Workspace ID | Sim | UUID do workspace no Castnexo |
| Desativar a decoração de links de checkout | Não | A decoração (Hotmart, Kiwify e similares) vem ativada; marque para desativar |
| Cookie de vínculo do checkout | Não | Usado quando a decoração está desativada |
| Parâmetro de origem na URL do checkout | Não | Usado quando a decoração está desativada (padrão: `src`) |
| Eventos do dataLayer a capturar | Não | Eventos personalizados do dataLayer (os eventos padrão já são capturados automaticamente) |
| Domínios para vínculo cross-domain | Não | Lista de domínios envolvidos no fluxo cross-domain (mesmo cliente em domínios diferentes). Liste todos, incluindo o domínio atual. O tracker precisa estar instalado em todos os domínios listados |
| Timeout de sessão | Não | Em milissegundos (padrão: 1800000) |
| Validade dos UTMs | Não | Em dias (padrão: 7) |
| Modo debug | Não | Logs no console do navegador |

## Permissões

| Permissão | Escopo |
|-----------|--------|
| Injects Scripts | Restrita a `https://tracker.castnexo.com.br/script/latest.js` |
| Accesses Global Variables | Variáveis de configuração com prefixo `__GM_` (somente escrita) |

## Privacidade e tratamento de dados

Este template carrega um script de **analytics** que coleta dados de
comportamento de navegação (visualizações de página, cliques, rolagem, envios
de formulário, dados de sessão e de dispositivo) e dados de atribuição de
tráfego. O uso exige uma conta Castnexo e os dados são processados conforme a
Política de Privacidade do Castnexo:
<https://tracker.castnexo.com.br/privacy>.

O responsável pelo site deve garantir a base legal e o consentimento
adequados antes de ativar a coleta.

## Licença

Apache License 2.0 — ver [LICENSE](LICENSE).

## Autor

Desenvolvido por Vinicius Castilho — [castnexo.com.br](https://castnexo.com.br)
