# Afrofuturismo — CEPI Marajó

Site estático para GitHub Pages. Público: 8º e 9º anos. Visualização sem conta; login Google para votar e administrar.

## Estado da integração

A página está pronta para apresentação. A conexão Firebase está desativada em `firebase-config.js` até a aprovação do projeto de destino e publicação de suas regras. Nenhuma alteração de regras foi aplicada nesta entrega.

Projeto proposto: `leciona-eaa56`, o projeto referenciado pelo Amefricanidades. Nó separado: `afrofuturismo_2026`.

## Ativação

1. Ler as regras atualmente implantadas no console do Firebase.
2. Acrescentar apenas o nó de `database.rules.fragment.json` em `rules`, preservando os demais projetos. Não substituir as regras completas pelo fragmento.
3. Confirmar Google como provedor de autenticação e `malucesarrobot.github.io` como domínio autorizado.
4. Alterar `enabled` para `true` em `firebase-config.js`.
5. Testar com a conta `malu.cesar@gmail.com`: importar uma turma, cadastrar um desenho e conferir em outro dispositivo.

Os nomes da relação ficam restritos à administradora. A galeria mostra número, turma e obra. Imagens são convertidas em JPEG e compactadas antes do envio ao Realtime Database.

Voto único por UID Google e categoria, com criação imutável protegida nas regras. Período: 10/11/2026 00h a 15/11/2026 23h59min59s, horário de Brasília. Apuração pública após publicação da professora em 18/11. Exclusão de desenho bloqueada a partir do início da votação.

Um usuário com múltiplas contas Google ainda pode votar por contas distintas; isto é controle por conta, não comprovação de identidade civil.

## Código-fonte

Os arquivos da aplicação estão em `source`. Para reconstruir: instalar React, React DOM, lucide-react, Vite e @vitejs/plugin-react; executar `vite build`; copiar a saída para esta pasta preservando as regras. Os SDKs Firebase compat são compartilhados com a pasta `../vendor` já existente no repositório.
