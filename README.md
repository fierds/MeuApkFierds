# Vendas em Dia

Aplicativo pessoal para registrar vendas dos produtos de R$ 120 e R$ 50, recebimentos, pendências e saídas. Tema preto AMOLED.

## Recursos
- Cadastro de vendas com cliente, data, forma de pagamento e valor recebido.
- Baixa parcial ou total de pagamentos.
- Registro e exclusão de saídas/despesas.
- Resumo geral e relatórios dos últimos 7 dias ou do mês atual.
- Exportação CSV.
- Dados armazenados localmente no dispositivo; sem conta e sem Supabase.

## Executar
```sh
npm install
npm run dev
``

## Gerar APK Android sem Play Store
Instale Node.js, Android Studio e o SDK Android. Depois:
```sh
npm install
npm run build
npx cap add android
npx cap sync android
npx cap open android
``
No Android Studio, use **Build > Build Bundle(s) / APK(s) > Build APK(s)**. O APK pode ser instalado diretamente no seu aparelho. Para atualizar, rode novamente `npm run build` e `npx cap sync android`, e gere outro APK.

## Dados e privacidade
Os dados ficam no armazenamento local do aplicativo. Limpar os dados ou desinstalar pode apagar os registros. Exporte CSV regularmente e guarde uma cópia. Não há sincronização entre aparelhos.
