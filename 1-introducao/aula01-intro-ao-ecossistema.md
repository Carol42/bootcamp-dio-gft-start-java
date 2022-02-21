# Introdução ao Ecossistema e Documentação Java
Curso ministrado por [Daniel Hatanaka](https://github.com/hatanakadaniel)

## Aula 01 - Introdução ao Ecossistema Java

#### O que é Java?
"Java é uma linguagem de programação e plataforma computacional lançada pela primeira vez pela Sun Microsystems em 1995". Oracle, 2021. Disponível em: <<https://www.java.com/pt-BR/download/help/whatis_java.html>>

#### Características da Linguagem Java:

- Compilada;
- Interpretada;
- Fortemente tipada;
- Linguagem de alto nível;
- Executada em uma máquina virtual - JVM (Java Virtual Machine).


#### O que é a JVM?
"JVM (Java Virtual Machine) é uma máquina virtual responsável pela tradução dos *ByteCodes* oriundos do compilador **Javac (Java Compiler)** em código de máquina de cada sistema operacional."

#### Características da JVM:
- Execução de pilhas;
- Gerenciamento de memória;
- Gerenciamento de threads;
- Otimização de código (Compilação JIT - Just In Time);
- Garbage Collector (GB).

#### Diferenças entre JRE e JDK

- **JRE (Java Runtime Environment)** - responsável por executar os programas em Java.
- **JDK (Java Development Kit)** - utilitários que permite o desenvolvimento de programas em Java. Já possui a JVM para executar os programas.

#### Tipos de plataformas Java

- **Java SE (Java Standard Edition)** - contém as especificações do Java e pode ser implementado por diversas empresas como Oracle, OpenJDK, Azul Zulu, etc.
- **Java EE (Java Enterprise Edition)** - contém todas as especificações do Java SE e um número de programas úteis para que executem em servidores. Em 2019 foi renomeado para Jakarta EE. Utilizado em desenvolvimento web.
- **Java ME (Java Micro Edition)** - contém especificações para desenvolvimento de programas para dispositivos pequenos como celulares, PDAs, sistemas embarcados, entre outros.

#### Implementações Java SE
- **OpenJDK**
- OracleJDK
- AdoptOpenJDK
- Amazon Corretto
- GraalVM CE
- Azul Zulu

#### Instalando a JVM
Podemos instalar o Java diretamente do repositório do Sistema Operacional. Porém, como pode ser que precisemos de outras versões do Java dependendo do projeto em que estamos trabalhando, é interessante instalar utilizando um Gerenciador de Versões do Java, que permite trocarmos de versão com facilidade.

Nesse curso utilizamos o Jabba. Para instalar o JDK utilizando o Jabba, basta rodar o seguinte comando no terminal:

```bash
curl -sL https://github.com/shyiko/jabba/raw/master/install.sh | bash && . ~/.jabba/jabba.sh
```

#### Utilizando o Java Version Manager

```bash
# lista todas as versões do JDK
jabba ls-remote

# instala a versão indicada
jabba install openjdk@1.11

# para usar a versão indicada:
jabba use openjdk@1.11

# verifica qual versão do java está sendo usada
java -version
```
