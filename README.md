# Golang com Graphql - School of net

Fundamentos do GraphQL e como implementar com a lib gqlgen - https://gqlgen.com/


## 🧑‍💻 query!

```sh
query findCategories {
  categories {
    id
    name
    description
    courses {
      id
      name
    }
  }
}

query findCourses {
  courses {
    id
    name
    description
    category {
      id
      name
      description
    }
    chapters {
      id
      name
    }
  }
}

query findChapters {
  chapters {
    id
    name
    course {
      id
      name
      category {
        id
        name
      }
    }
  }
}
```

## 🧑‍💻 mutations!
```sh
mutation createCategory {
  createCategory(input: { name: "Go", description: "Go is awesome" }) {
    id
    name
    description
  }
}

mutation createCourse {
  createCourse(
    input: {
      name: "Go Advanced"
      description: "Go advanced"
      categoryID: "T5577006791947779410"
    }
  ) {
    id
    name
    description
    category {
      id
      name
    }
  }
}

mutation createChapter {
  createChapter(
    input: { name: "GO - Chapter 1", courseId: "T8674665223082153551" }
  ) {
    id
    name
    course {
      name
    }
  }
}
```
## Contatos

[![Github Badge](https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/wander4747)](https://github.com/wander4747)
[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/wander-douglas/)](https://www.linkedin.com/in/wander-douglas/)
[![Whatsapp Badge](https://img.shields.io/badge/-Whatsapp-4CA143?style=flat-square&labelColor=4CA143&logo=whatsapp&logoColor=white&link=https://api.whatsapp.com/send?phone=5531993326096&text=Hello!)](https://api.whatsapp.com/send?phone=5531993326096&text=Hello!)
[![Gmail Badge](https://img.shields.io/badge/-Gmail-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:wander.douglas14@gmail.com)](mailto:wander.douglas14@gmail.com)

Feito com muito ❤️☕👨🏻‍💻 por Wander Douglas