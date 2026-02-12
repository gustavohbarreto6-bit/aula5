# aula5
📅 Calculadora de Intervalos entre Datas

Projeto web simples desenvolvido com HTML, CSS e JavaScript, que permite calcular o intervalo entre duas datas informadas pelo usuário, exibindo o resultado em dias, meses (aproximado) e anos (aproximado).

🚀 Funcionalidades

Inserção de duas datas através de campos do tipo date

Cálculo automático da diferença entre as datas

Exibição do resultado em:

✅ Dias

✅ Meses (aproximadamente)

✅ Anos (aproximadamente)

Validação para impedir cálculo com campos vazios

Botão para limpar os campos e redefinir o resultado

🗂 Estrutura do Projeto
📁 projeto/
│
├── index.html   # Estrutura da página + lógica JavaScript
└── style.css    # Estilização da interface

🧠 Como Funciona
1️⃣ Captura das Datas

O sistema coleta os valores inseridos nos campos:

const data1 = document.getElementById("data1").value;
const data2 = document.getElementById("data2").value;

2️⃣ Validação

Se algum campo estiver vazio, uma mensagem de erro é exibida na tela.

3️⃣ Cálculo da Diferença

Converte as datas para objetos Date

Calcula a diferença em milissegundos

Converte para dias

Converte dias para meses (divisão por 30)

Converte meses para anos (divisão por 12)

const diffEmDias = Math.floor(diffEmMs / (1000 * 60 * 60 * 24));


⚠️ Observação: Meses e anos são valores aproximados.

🎨 Estilização

O arquivo style.css define:

Fundo azul claro

Layout centralizado

Botões com efeito hover

Caixa de resultado com sombra e bordas arredondadas

Interface limpa e organizada

🖥 Como Executar

Baixe os arquivos:

index.html

style.css

Coloque ambos na mesma pasta.

Abra o arquivo index.html no navegador.

Não é necessário servidor ou instalação adicional.

📌 Tecnologias Utilizadas

HTML5

CSS3

JavaScript (Vanilla JS)

💡 Possíveis Melhorias Futuras

Cálculo exato de meses e anos

Layout responsivo mais avançado

Separar o JavaScript em arquivo próprio (script.js)

Animações suaves no resultado

Validação para datas iguais ou futuras
