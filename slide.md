---
marp: true
theme: academic-erbase
paginate: true
math: katex
---

<!-- _class: lead -->

![top-right](https://main--ornate-begonia-abfe87.netlify.app/assets/logo.svg)

## Elaboração de materiais didáticos com Marp e CI/CD

**AUTORES**: Reinan Gabriel Dos Santos Souza
Prof. MSc. Francisco Rodrigues Santos
Prof. Dr. Gilson Pereira Dos Santos Junior

<!-- _footer: '07 de novembro de 2024' -->

---

![bg left:40% 80%](https://www.qrtag.net/api/qr_1280.png?url=https://reinanhs.github.io/marp-erbase-presentation/)

**Material utilizado na apresentação**

Todos os materiais relacionados à apresentação estão disponíveis digitalmente no meu repositório do **GitHub**. Para acessar esses recursos, basta escanear o **QR Code** na imagem ao lado.

> https://github.com/ReinanHS/marp-erbase-presentation

---

<!-- _header: Sumário -->

- Problema
- Objetivo geral
- Solução
- Resultados
- Conclusão
- Trabalhos futuros
- Principais referências

---

<!-- _header: PROBLEMA -->

1. **Carência de automatização** na elaboração de materiais didáticos;
2. **Dificuldade em manter** e atualizar materiais didáticos;
3. **Falta de padronização** nos materiais didáticos;
4. **Complexidade** na utilização de códigos e fórmulas matemáticas.

---

<!-- _header: OBJETIVO GERAL -->

Apresentar uma abordagem para a elaboração de materiais didáticos **simples**, **flexíveis** e em **múltiplos formatos** utilizando o Marp ¹.

![w:500 center](https://raw.githubusercontent.com/ReinanHS/marp-erbase-presentation/refs/heads/master/img/ilustracao_objetivos.png)

<!-- <c>Fonte: Autor, (2024).</c> -->

> ¹ https://marp.app/

---

<!-- _class: image_with_font -->
<!-- _header: SOLUÇÃO  -->

![w:1000 center](https://gitlab.com/reinanhs/repo-slide-presentation/-/raw/main/imagens/tcc/exemplo-do-marp-slide.png)

Fonte: Autor, (2024).

---

<!-- _class: image_with_font -->
<!-- _header: EXEMPLO DE ESCRITA DO SLIDE EM MARKDOWN  -->

![w:1200 center](https://raw.githubusercontent.com/ReinanHS/marp-erbase-presentation/refs/heads/master/img/exemplo-vetor.png)

Fonte: Autor, (2024).

---

<!-- _header: EXEMPLO DE BLOCO DE CÓDIGO  -->

A documentação oficial do **Marp** ² suporta blocos de código em várias linguagens. Veja o exemplo abaixo:

```python
idade = input('qual a sua idade? ')
print ('%d anos' %idade)

numeros = (1,2,3,4,5,6)

for i in numeros:
    print(i)
```

> ² https://github.com/marp-team/marp-core?tab=readme-ov-file#auto-shrink-the-block

---

<!-- _header: EXPRESSÕES MATEMÁTICAS  -->

Segundo Arino (2022), o Marp permite escolher entre o **MathJax** e o **KaTeX**. Veja o exemplo abaixo:

```tex
\begin{align*}
S(\omega) 
&= \frac{\alpha g^2}{\omega^5} \exp\left[ -0.74 \left\{ \frac{\omega U_\omega}{19.5 g} \right\}^{\!-4} \right] \\
&= \frac{\alpha g^2}{\omega^5} \exp \left[ -0.74 \left\{ \frac{\omega U_\omega}{19.5 g} \right\}^{-4} \right]
\end{align*}
```

$$
\begin{align*}
S(\omega) 
&= \frac{\alpha g^2}{\omega^5} \exp\left[ -0.74 \left\{ \frac{\omega U_\omega}{19.5 g} \right\}^{\!-4} \right] \\
&= \frac{\alpha g^2}{\omega^5} \exp \left[ -0.74 \left\{ \frac{\omega U_\omega}{19.5 g} \right\}^{-4} \right]
\end{align*}
$$

> https://julien-arino.github.io/blog/2022/Marp-for-slides/

---
<!-- _header: PIPELINE PARA AUTOMATIZAR A COMPILAÇÃO E PUBLICAÇÃO -->

Veja abaixo o exemplo do fluxo de execução da pipeline ³:

![w:900 center](https://gitlab.com/reinanhs/repo-slide-presentation/-/raw/main/imagens/tcc/github-action-pipeline.png)

<!-- <c>Fonte: Autor, (2024).</c> -->

> ³ https://github.com/ReinanHS/limarka-template-tcc/actions/runs/10801707397

---
<!-- _class: image_with_font -->
<!-- _header: RESULTADO DA PÁGINA DE PUBLICAÇÃO GERADO PELO CI/CD -->

![w:650 center](https://gitlab.com/reinanhs/repo-slide-presentation/-/raw/main/imagens/tcc/limarka-page.png)

Fonte: Autor, (2024).

> Link para a página: https://reinanhs.github.io/limarka-template-tcc/
> Link para o Limarka Page: https://github.com/ReinanHS/limarka-render-html

---

<!-- _header: CONCLUSÃO -->

- Facilidade e automação na criação de materiais didáticos.
- Otimização do tempo com automação de publicação e compilação.
- Acesso simplificado ao conteúdo por meio de uma página web.
- Flexibilidade na distribuição em múltiplos formatos.

---

<!-- _header: TRABALHOS FUTUROS -->

- Ampliar a acessibilidade dos materiais didáticos gerados com Marp, focando em necessidades especiais.
- Avaliar o impacto do uso de Marp e CI/CD na melhoria do engajamento dos alunos.
- Realizar a implementação de novas validações no CI.

---

<!-- _header: PRINCIPAIS REFERÊNCIAS -->

**ARINO, Julien (2022)**. Marp for slides. Disponível em: https://julien-arino.github.io/blog/2022/Marp-for-slides/. Acesso em: 30 out. 2024.
**Marp (2024)**. Markdown presentation ecosystem. Disponível em: https://marp.app/. Acessado em: 23 out. 2024.
**Tenen, D. and Wythoff, G. (2022)**. Autoria sustentável em texto simples usando pandoc e markdown. The Programming Historian em Português.
