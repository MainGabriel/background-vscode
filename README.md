<h1>Como colocar background no Vscode</h1>
<h3>Eu só conseguir colocar animação que foram baixadas da página pin page:</h3>

-instale a extension no vscode 'Custom css and Js Loader'
- crie o diretório C:\Users\[seu usuario]\.vscode\vscode_style\vscode_style.css
- adicione esse css no arquivo vscode_style.css
  
```
  body{
  pointer-events: auto !important;
  background-size: 100% !important;
  opacity: 0.90 !important;
  background-position: 0 0 !important;
  background-image: url(https://raw.githubusercontent.com/MainGabriel/background-vscode/master/background-galaxy.gif);
  content: '';
  position: absolute;
  z-index: 999;
  width: 100%;
  background-repeat: no-repeat;
  }
```
- vai na configuração do vscode: atalho ctrl + shift + p e procure por settings e procure por "code actions on save" e click em "Edit in settings.json" para abrir o arquivo conforme imagens:
  <p><img src="https://github.com/MainGabriel/background-vscode/blob/master/config/config-vscode.png" width=550px> </p>
  <p><img src="https://github.com/MainGabriel/background-vscode/blob/master/config/config-vscode-1.png" width=550px/></p>
      
- após isso acrescente o código
```
"vscode_custom_css.imports":["file:///C:/Users/dev_g/.vscode/vscode_style/vscode_style.css"],
```
  <img src="https://github.com/MainGabriel/background-vscode/blob/master/config/config-vscode-2.png" width=550px/>
  
- depois dessas configurações, apenas colocar a imagem ou animação desejada adicionando a imagem/animação no arquivo que está no caminho "C:\Users\[seu usuario]\.vscode\vscode_style\vscode_style.css" na propriedade: background-image: url();
- Depois de ter colocado a imagem no arquivo "vscode_style.css", no vscode com o atalho "ctrl + shift + p" procure por "Enable Custom CSS and Js" e click, vai pedi para restartar o vcode e quando voltar vai aparecer a imagem de fundo
 
<img src="https://github.com/MainGabriel/background-vscode/blob/master/config/enable-image.png" width=550px/>
- Depois de feito, se quiser substituir a imagem/animação apenas troque o caminho no arquivo vscode_style.css e procure por "Reload Custom CSS and Js" para mudar o background

<img src="https://github.com/MainGabriel/background-vscode/blob/master/config/reload-image.png" width=550px/>
 <h5>Como procurar: </h5>
   
- pesquise por "ping page gif [nome da animação que quer, por exemplo: 'ping page gif star wars']"
- suba essa imagem no repositório no github
