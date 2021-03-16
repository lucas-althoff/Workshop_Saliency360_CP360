Descrever em poucas palavras como foi o estudo de PySaliency. Utilizem os recursos do MarkDown.
- [Tutorial](https://www.markdowntutorial.com/)

# Myllena

## Ambiente
* JupyterLab instalado pelo anaconda.
* Windows 10

## Problemas com Pysaliency
### Problema com ferramentas de c++
  * São necessária [feramentas de compilação de c++](https://visualstudio.microsoft.com/pt-br/visual-cpp-build-tools/) para instalar a pysaliency 
  * Problema com arquivo .pyx Solução [Stackoverflow:](https://stackoverflow.com/questions/7508803/how-do-i-import-function-from-pyx-file-in-python)
  
  `import pyximport`
  
  `pyximport.install()`
              
  * Problema encontrado:
     ImportError: Building module pysaliency.roc failed: ["distutils.errors.CompileError: command 'C:\\\\Program Files (x86)\\\\Microsoft Visual Studio\\\\2019\\\\BuildTools\\\\VC\\\\Tools\\\\MSVC\\\\14.28.29910\\\\bin\\\\HostX86\\\\x64\\\\cl.exe' failed with exit status 2\n"]

### Instalar Matlab
  * Matlab ainda está em processo de instalação. Preferi tentar instalar uma vez que outros datasets precisam.


# Israel
## Ambientes testados
* Notebooks em Colab
* Jupyter notebook por anaconda
* Diretamente do terminal do python

## Problemas
### Colab
É necessária a importação de bibliotecas que não existem

### Jupyter notebook
O kernel utilizado no código é de Python 2.7, o que impede a compilação correta em Jupyter. Olhando a documentação do Py 2.7 explica-se o motivo das bibliotecas não serem achadas em colab

### Local pelo terminal
É explicado no git do projeto como instalar diretamente por pypi. Quando tentei instalar, tive problema com o comando pip que eu não pude resolver antes da reunião.

## Situação atual
Download de novo algoritmo a ser rodado em MATLAB e estudo de artigos na área em busca de bons algoritmos.
