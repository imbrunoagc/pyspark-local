Projeto Pyspark Local
Este projeto configura um ambiente local para utilizar o PySpark de forma eficiente. Siga as instruções abaixo para configurar seu ambiente.

### **Requisitos**
1. **WSL** (Windows Subsystem for Linux)
Certifique-se de ter o WSL instalado e configurado no seu sistema Windows.

2. **Java**
Instale o Java nas versões 11 ou 17.

3. **Apache Spark**
Baixe e instale o Apache Spark compatível com sua versão do Hadoop.

4. **winutils.exe**
Como o Windows não suporta o Hadoop nativamente, é necessário instalar um programa para conseguir executar o Hadoop na sua máquina.

5. **Configuração das Variáveis de Ambiente**
Configure as seguintes variáveis de ambiente no seu sistema:

* **JAVA_HOME**: Caminho para o diretório de instalação do Java.
```bash
JAVA_HOME=C:\Arquivos e Programas\Java\jdk\bin
```

* **HADOOP_HOME**: Caminho para o diretório de instalação do Hadoop/Spark.
```bash
HADOOP_HOME=C:\hadoop\spark_version
```

* **SPARK_HOME**: Caminho para o diretório de instalação do Spark.
```bash
SPARK_HOME=C:\spark\spark_version
```

### **Passos de Instalação**

1. Verificar a Instalação do Java
Abra o terminal e execute:
```bash
java -version
```
*Certifique-se de que a versão exibida corresponde à versão instalada (11 ou 17).*

2. Verificar a Instalação do Spark
No terminal, execute:
```bash
pyspark
```
Isso deve iniciar o shell do PySpark, indicando que o Spark está instalado corretamente.

## **Gerenciamento de Pacotes com Poetry**
Utilizamos o Poetry como gerenciador de pacotes do Python para isolar as dependências por projeto.

**Bibliotecas Utilizadas**
* ***PySpark:*** Processamento e uso do Spark com Python.
* ***JupyterLab:*** Interface gráfica interativa do Jupyter para desenvolvimento e visualização.

## ***Uso***
***Iniciar o JupyterLab***
Para acessar o ambiente do JupyterLab, execute o seguinte comando no terminal:
```bash
jupyter lab
```
Isso abrirá a interface gráfica interativa do JupyterLab no seu navegador, onde você pode executar comandos em Spark.

**Diferencial:** Este projeto não utiliza o Anaconda. Em vez disso, utilizamos o Python puro e a biblioteca jupyter-lab para acessar a interface e executar comandos no Spark.

Material de Apoio
Para mais detalhes sobre a instalação e configuração do PySpark no Windows para conexão com o Azure Data Lake, consulte o [artigo de apoio]('https://medium.com/@bruno.facco/instala%C3%A7%C3%A3o-e-configura%C3%A7%C3%A3o-do-pyspark-no-windows-para-conex%C3%A3o-no-azure-datalake-f166351da69e').

Contribuição
Sinta-se à vontade para contribuir com este projeto abrindo issues ou enviando pull requests.