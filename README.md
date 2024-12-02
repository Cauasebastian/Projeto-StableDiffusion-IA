# Geração de Imagem com IA (Disciplina de INTELIGENCIA ARTIFICIAL APLICADA)
 
Este projeto utiliza o modelo de difusão Stable Diffusion para gerar imagens a partir de prompts textuais. O modelo é otimizado para criar imagens de alta qualidade, baseadas em descrições detalhadas fornecidas pelo usuário. O sistema permite a escolha de diferentes versões do modelo, ajuste de parâmetros, e a aplicação de estilos gráficos.

## Tecnologias Utilizadas

- Gradio: Para criação da interface gráfica.
- Stable Diffusion: Para geração de imagens a partir de texto.
- Torch: Para processamento eficiente com GPU.
- Diffusers: Biblioteca para manipulação de modelos de difusão.

## Funcionalidades

- Geração de Imagens: O usuário pode fornecer um prompt textual para gerar uma imagem. A descrição pode ser ajustada para fornecer resultados mais específicos ou criativos.
- Modelos Diversos: O sistema suporta várias versões do modelo Stable Diffusion (1.5, 2.1), e também modelos adicionais como o Lightning V4.0 e Lightning V5.0 (opcionais).
- Parâmetros Configuráveis:
- Prompt: Descrição detalhada da imagem que será gerada.
- Prompt Negativo: O que não deve aparecer na imagem.
- Estilo de Imagem: Resolução e detalhamento da imagem gerada.
- Seed: Para garantir a mesma imagem com o mesmo prompt.
- Escalamento de Orientação: Intensidade com que o modelo segue o prompt.
- Passos de Inferência: Controle sobre o número de passos de cálculo para maior ou menor detalhamento.

## Como usar 
1. Instalação: Para usar este sistema, você precisa instalar as dependências necessárias. Você pode fazer isso executando o seguinte comando:
 ```python
  !pip install diffusers torch torchvision pipeline transformers accelerate safetensors sentencepiece spaces peft 
  ```
2. Execução: Após a instalação, execute o script principal para iniciar a interface Gradio:
```python
   python app.py
```
3. Interface: A interface Gradio será aberta no seu navegador. Nela, você pode:
   - Inserir um prompt descritivo da imagem.
   - Escolher o modelo de difusão e estilo de imagem.
   - Ajustar os parâmetros como seed, passos de inferência, e escala de orientação.
   - Gerar a imagem desejada.
4. Exemplos de Prompt: Aqui estão alguns exemplos de prompts para você testar:
   - "A futuristic cityscape with neon lights and flying cars, cyberpunk theme, 4k, ultra-detailed"
   - "A majestic lion standing on a rocky cliff during sunset, hyper-realistic, 4K resolution"
   - "A cozy winter cabin with a fireplace glowing warmly, snow falling outside, peaceful atmosphere"
   - "A surreal dreamscape with floating islands and vibrant flowers, ethereal theme, vibrant colors"
5. Visualização: Após gerar a imagem, ela será exibida na interface e estará disponível para download.
## Parâmetros de Geração

- Modelo: Escolha entre "Stable Diffusion 1.5" e "Stable Diffusion 2.1".
- Estilo: Selecione o estilo de imagem, como 3840 x 2160 (8K), 2560 x 1440 (4K), ou 2K.
- Seed: Use um número específico ou deixe aleatório para gerar imagens diversas.
- Número de Imagens: Ajuste para gerar múltiplas imagens de uma vez.
- Tamanho da Imagem: Defina a largura e altura da imagem gerada.
- Escalamento de Orientação: Determine a fidelidade da imagem ao prompt.

## Modelos Disponíveis
1. Stable Diffusion 1.5: Ideal para imagens mais clássicas e balanceadas.
2. Stable Diffusion 2.1: Gera imagens mais nítidas e detalhadas.
3. Stable Diffusion 3.5-large-turbo: Modelo avançado com melhor entendimento semântico dos prompts.
4. Lightning V4.0 e V5.0: Modelos especializados para imagens com maior realismo e controle sobre os detalhes.

## Modelos Disponíveis

### Stable Diffusion 1.5
- Menor capacidade de detalhamento, mais criativo e rápido.
- Ideal para imagens clássicas e de alta qualidade.
### Stable Diffusion 2.1
- Maior capacidade de detalhamento e refinamento de imagens.
- Ideal para gerar cenas realistas e complexas.
### Stable Diffusion 3.5-large-turbo
- Modelo avançado com maior fidelidade nos detalhes e relações contextuais.
- Ideal para imagens com detalhes complexos e abstrações.
### Lightning V4.0 e V5.0
- Modelos avançados com 1,5 a 3 bilhões de parâmetros.
- Produzem imagens altamente realistas e com grande controle sobre os elementos do prompt.

## Contribuindo
Se você deseja contribuir com este projeto, por favor, siga estas etapas:

1. Faça um fork do repositório.
2. Crie uma branch com suas modificações (git checkout -b feature-nome).
3. Commit suas alterações (git commit -am 'Adicionar nova funcionalidade').
4. Faça o push para a branch (git push origin feature-nome).
5. Crie um novo pull request.
