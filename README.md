<h1 align="center"> Gerador de QR Code </h1>

<p align="center">
Um projeto simples em **HTML, CSS e JavaScript** que permite gerar códigos QR a partir de um texto ou URL inserido pelo usuário.
</p>

<p align="center">
  <a href="#-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

<p align="center">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT&color=49AA26&labelColor=000000">
</p>

<br>

## 🚀 Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:

- **HTML** — estrutura da página  
- **CSS** — estilos e layout  
- **JavaScript** — lógica de geração do QR Code  

## 💻 Projeto

Um projeto simples em **HTML, CSS e JavaScript** que permite gerar códigos QR a partir de um texto ou URL inserido pelo usuário.

A aplicação usa a API pública `api.qrserver.com` para gerar a imagem do QR Code de forma rápida e sem dependências extras.

## 🚀 1. Funcionalidade

- ✔️ Aceita texto ou endereço de URL  
- ✔️ Gera QR Code baseado no valor digitado  
- ✔️ Mostra a imagem gerada diretamente na página  

---

## 🧠 2. Como funciona

Quando o usuário insere um texto ou link e clica em **Gerar QR Code**, o JavaScript atualiza a imagem (`<img>`) utilizando a API:

```
https://api.qrserver.com/v1/create-qr-code/?size=170x170&data=SEU_TEXTO
```

A imagem é carregada dinamicamente com o QR Code gerado.

---

## 💡 3. Exemplo de código principal

```js
generateBtn.addEventListener('click', () => {
  let qrValue = qrInput.value;
  if (!qrValue) {
    alert('Insira uma URL ou texto para gerar um QR Code')
    return;
  }
  generateBtn.innerText = 'Gerando um QR Code...'
  qrImg.src = `https://api.qrserver.com/v1/create-qr-code/?size=170x170&data=${qrValue}`;
});
```

---

## :memo: Licença

Esse projeto está sob a licença MIT.
