# React Input por Extenso

Componente React que retorna número por extenso

[![npm](https://img.shields.io/npm/v/react-input-por-extenso)](https://www.npmjs.com/package/react-input-por-extenso) ![NPM](https://img.shields.io/npm/l/react-input-por-extenso)

## Como instalar

Abaixo as formas de como instalar essa biblioteca utilizando o npm ou yarn:

```
npm install react-input-por-extenso
# ou
yarn add react-input-por-extenso
```

## Como usar

Uma forma básica de como utilizar o componente:

```jsx
import React, { useState } from "react";
import ReactDOM from "react-dom";
import ReactInputPorExtenso from "react-input-por-extenso";

const App = () => {
  const [numero, setNumero] = useState("");

  return (
    <>
      <ReactInputPorExtenso
        tipoExtenso="monetario"
        onChange={numeroExtenso => setNumero(numeroExtenso)}
      />
      <p>
        <strong>Número por extenso</strong>: {numero}
      </p>
    </>
  );
};

ReactDOM.render(<App />, document.getElementById("root"));
```

## Propriedades

Esse componente é uma abstração de um componente input do tipo numérico,
todas as propriedades de um input estão disponíveis.

| Propriedade | Valor inicial | Tipo   | Descrição                     |
| ----------- | ------------- | ------ | ----------------------------- |
| tipoExtenso | normal        | string | Formato de extensão do número |
