# Introdução ao Ecossistema e Documentação Java
Curso ministrado por [Daniel Hatanaka](https://github.com/hatanakadaniel)

## Aula 03 - Documentação Java

#### Comentários
Comentários em linha são feitos utilizando ```//``` no começo:
```java
// esse é um comentário em linha no Java!
```
Comentários em bloco são feitos utilizando ```/**``` no começo e ```*/``` no final:
```java
/**
 * Esse é um comentário
 * Em bloco
 * Na linguagem Java!
 * /
```

#### Javadoc
É uma ferramenta para documentação no formato HTML que se baseia nos comentários do código-fonte. Os comentários precisam conter tags para que a documentação fique legível.

#### Tags Javadoc

- @author - especifica o autor da classe ou do método
- @deprecated - identifica classes ou métodos obsoletos
- @link - possibilita a definição de um link para um outro documento local ou remoto através de uma URL
- @param - descreve um parâmetro que será passado a um método
- @return - descreve qual o tipo de retorno do método
- @see - associa a outras classes ou métodos
- @since - descreve desde quando uma classe ou método foi adicionado
- @throws - descreve os tipode de exceções que podem ser lançadas por um método
- @version - descreve a versão da classe ou do método

#### Comando para gerar os arquivos da documentação
```bash
javadoc -d javadoc/ -sourcepath src/ -subpackages com.dio
```