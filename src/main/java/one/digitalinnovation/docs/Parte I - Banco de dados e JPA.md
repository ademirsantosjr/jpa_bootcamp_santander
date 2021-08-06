# Banco de dados e JPA
* JPA
* Implementações JPA
    + Hibernate
    + EclipseLink
* Linguagens de consulta orientada a objetos
## JPA
* Maior produtividade trabalhar com SQL e JDBC
* Lidar com paradigmas diferentes:
    + Orientação a objetos (Java)
    + Entidade relacional (SGBD)
## Surge ORM
* ORM: Mapeamento Objeto Relacional
* Traduz objeto em entidade relacional
    + Tabela - Classe
    + Coluna - Atributo
    + Registro - Objeto
## Java Persistence API (JPA)
* Especificação oficial chamada JPA
* Descreve como frameworks ORM deve se comportar
* A JPA sozinha não permite executar operações entre aplicação e BD.
## Recurso
* javax.persistence
## Artefatos importantes
* `@Entity` - indica que o objeto da classe será persistido em banco de dados
* `@id`, `@column`, `@table`, `@OneToMany`, `@ManyToOne`
* Interface `EntityManager` - gerencia ciclos de vida das entidades
    + métodos: `find`, `persist`, `remove`
## Uso do JPA
* JPA usa JDBD por baixo dos panos
    + baixar JPA e driver JDBC via ferramenta de build
* Criar `persistence.xml`: URL de conexão, usuário, senha, driver e classes que serão mapeadas.
* Utilizar _annotations_ nas classes mapeadas para uso posterior do Hibernate
* Configurar `entityManager`