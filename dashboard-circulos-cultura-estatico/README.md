# Dashboard GEEJA — Círculos de Cultura

Versão 100% estática do dashboard, conectada diretamente à planilha Google Sheets.

## Características
- Sem banco de dados.
- Sem função serverless.
- Sem dependência da Vercel.
- Atualização automática a cada 60 segundos.
- Botão de atualização manual.
- Filtros e gráficos gerados a partir dos dados da planilha.
- Galeria baseada na coluna `Insira aqui fotos do encontros`.
- Compatível com GitHub Pages, Cloudflare Pages, Netlify e hospedagem estática equivalente.

## Atualização dos dados
O navegador consulta diretamente a aba pública do Google Sheets usando a interface pública de visualização do Google. Quando a planilha é alterada, o dashboard reflete os novos dados na próxima atualização.

## Permissões necessárias
A planilha deve estar configurada para visualização por **qualquer pessoa com o link**.

Para que miniaturas de imagens do Google Drive apareçam para qualquer visitante, os arquivos correspondentes também precisam estar compartilhados para visualização pública. Caso contrário, o link do arquivo continuará disponível, mas a miniatura pode não carregar.

## GitHub Pages
1. Crie um repositório.
2. Envie `index.html`, `.nojekyll` e `README.md`.
3. Em **Settings > Pages**:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
4. Salve.

Não é necessário configurar variáveis de ambiente, build command ou banco de dados.
