# Pre-Processamento-PDF
Código para fazer pré-processamento de PDF's.

O que o código ajusta no PDF:
1. Aumenta a Nitidez 📈
Aplica um filtro de sharpening (kernel 3x3) em cada página
Deixa o texto e imagens mais claros e definidos

2. Corrige Orientação 🔄
Detecta se a página está de cabeça para baixo (rotacionada 180°)
Usa algoritmo ORB (detecção de features) para comparar a página normal vs rotacionada
Se detectar inversão, rotaciona automaticamente

3. Converte e Salva 💾
Lê o PDF página por página
Processa cada página individualmente
Salva como novo PDF com sufixo _processado.pdf
Mantém a qualidade (DPI 300 por padrão)

OBS: Serve apenas para PDF's com textos, para PDF's somente com imagens, será necessário utilizar OCR e nesse caso, é melhor utilizar Softwares como PDF24 ou até mesmo, baixar modelos de OCR locais como "Tesseract".
