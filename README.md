from PIL import Image, ImageDraw

# Crie uma nova imagem com um fundo branco
largura, altura = 800, 600
imagem = Image.new('RGB', (largura, altura), 'white')

# Crie um objeto de desenho
desenho = ImageDraw.Draw(imagem)

# Desenhe o céu azul
desenho.rectangle([(0, 0), (largura, altura // 2)], fill=(135, 206, 235))

# Desenhe a areia
desenho.rectangle([(0, altura // 2), (largura, altura)], fill=(244, 164, 96))

# Salve a imagem
imagem.save('praia.png')

# Exiba a imagem
imagem.show()

