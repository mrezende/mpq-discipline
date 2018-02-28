# Tese exemplo do IME USP 

Exemplo de tese/dissertação utilizado no IME USP. Este exemplo foi alterado para utilizar o encoding UTF-8. Ao invés de usar o pdflatex, estou utilizando xelatex.


Arquivo principal: 
  -'tese-exemplo.tex'

Arquivos dos capítulos e apêndice:
  - 'cap-introducao.tex'
  - 'cap-conceitos.tex'
  - 'cap-conclusoes.tex'
  - 'ape-conjuntos.tex'

Arquivo de bibliografia: 
  -'bibliografia.bib'

Diretório de figuras: 
  - './figuras/'
  
Compilação do documento:
  - make pdf : usando xelatex
  - make ps  : usando latex
  Ex:
      $ make pdf
  Obs: Para a compilação do documento que referencia figuras em formato 'ps' ou
       'eps' deve-se usar: 'make ps'
