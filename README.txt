# BodyTrack — PWA pessoal

Aplicativo pessoal para registrar peso, medidas corporais, alimentação, calorias, proteína, creatina e atividade física.

## Instalar no Android
Um PWA precisa ser servido por HTTPS para que o Chrome permita instalação e funcionamento offline (exceto localhost).
1. Extraia o ZIP.
2. Publique o conteúdo da pasta `bodytrack` em um host estático HTTPS, por exemplo GitHub Pages ou Netlify.
3. Abra o endereço HTTPS no Chrome do Android.
4. Menu ⋮ > **Instalar app** ou **Adicionar à tela inicial**.
5. Abra o BodyTrack uma vez online. Depois disso, a interface fica disponível offline.

## Dados e privacidade
- Os registros ficam no armazenamento local do navegador (`localStorage`) deste aparelho.
- Não há conta, servidor de banco de dados ou envio automático dos dados.
- Use Histórico > Exportar backup regularmente e guarde o JSON em local seguro.
- Para restaurar, use Importar backup.
- Limpar os dados do navegador ou desinstalar o app pode apagar registros locais. Faça backup antes.

## Desenvolvimento
Arquivos estáticos, sem dependências externas:
- `index.html`: interface e lógica.
- `manifest.webmanifest`: configuração PWA.
- `sw.js`: cache offline.
- `icons/`: ícones do app.

Metas iniciais pré-configuradas: 2.850 kcal, 125 g de proteína e 3 g de creatina. São referências editáveis na lógica do aplicativo, não prescrição nutricional.
