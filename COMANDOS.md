# Comandos do Projeto

Este projeto usa React com Vite.

## 1. Entrar na pasta do projeto

```powershell
cd "C:\Users\antun\OneDrive\Documentos\Codigo da faculdade\MIraki"
```

## 2. Instalar as dependencias

Use este comando na primeira vez, ou quando mudar o `package.json`:

```powershell
npm.cmd install
```

## 3. Rodar o projeto em desenvolvimento

```powershell
npm.cmd run dev -- --port 5173
```

Depois abra no navegador:

```text
http://127.0.0.1:5173
```

Se a tela parecer antiga ou em branco, aperte:

```text
Ctrl + F5
```

## 4. Gerar a versao final

```powershell
npm.cmd run build
```

O resultado sera criado na pasta:

```text
dist/
```

## 5. Testar a versao final localmente

```powershell
npm.cmd run preview -- --port 4173
```

Depois abra:

```text
http://127.0.0.1:4173
```

## 6. Pastas importantes

```text
src/
```

Onde fica o codigo React e o CSS principal.

```text
public/
```

Onde ficam as imagens, videos e logos usados pelo site.

```text
dist/
```

Pasta gerada automaticamente pelo build. Nao edite arquivos dentro dela.

```text
node_modules/
```

Dependencias instaladas pelo npm. Nao edite essa pasta.

## 7. Se a porta 5173 estiver ocupada

Rode em outra porta:

```powershell
npm.cmd run dev -- --port 5174
```

E abra:

```text
http://127.0.0.1:5174
```

## 8. Publicar no Render

Este projeto deve ser publicado como Static Site.

Antes de publicar, teste localmente:

```powershell
npm.cmd install
npm.cmd run build
```

No Render, use:

```text
Service Type: Static Site
Build Command: npm run build
Publish Directory: dist
```

Se usar Blueprint, o arquivo `render.yaml` da raiz ja configura isso automaticamente.
