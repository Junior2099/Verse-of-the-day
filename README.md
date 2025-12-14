# 📖 Site de Versículos Bíblicos

Site que exibe um versículo bíblico aleatório a cada atualização da página.

## 📋 Sobre os Versículos

O site foi configurado para buscar versículos de uma API online (bible-api.com), o que permite acessar **todos os versículos da Bíblia** (aproximadamente 31.173 versículos).

### Como Funciona

1. **Modo API (Recomendado)**: O site tenta buscar versículos aleatórios de uma API online que contém toda a Bíblia.
2. **Modo Local (Fallback)**: Se a API não estiver disponível, usa os 40 versículos incluídos localmente no arquivo `versiculos.js`.

## 🚀 Como Usar

1. Abra o arquivo `index.html` no seu navegador
2. Um versículo aleatório será exibido automaticamente
3. Atualize a página (F5) para ver um novo versículo
4. Use o botão "Novo Versículo" para ver outro sem recarregar a página
5. Use o botão "Compartilhar" para compartilhar ou copiar o versículo

## 📝 Adicionar Mais Versículos Localmente

Se quiser adicionar mais versículos ao arquivo local `versiculos.js`, edite o arquivo e adicione novos objetos ao array:

```javascript
{
    texto: "Seu versículo aqui",
    referencia: "Livro Capítulo:Versículo"
}
```

## ⚠️ Nota sobre a API

A API pode ter limitações de CORS quando acessada diretamente do navegador. Se isso acontecer:

1. Use um servidor local (ex: `python -m http.server` ou `npx serve`)
2. Ou adicione mais versículos ao arquivo `versiculos.js` localmente

## 🛠️ Executar com Servidor Local

Para evitar problemas de CORS com a API:

```bash
# Python 3
python3 -m http.server 8000

# Node.js (se tiver instalado)
npx serve

# PHP
php -S localhost:8000
```

Depois acesse: `http://localhost:8000`

