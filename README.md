<!-- README.md is generated from README.ecr, do not edit -->

# GraphQL server benchmarks

Graphql server benchmarks in many languages. Pull requests welcome, please read [CONTRIBUTING.md](CONTRIBUTING.md)

All servers implement a simple schema:

```graphql
type Query {
  hello: String!
}
```

The returned string is always `world`.

The API is served over HTTP using a common web server and load tested using [bombardier](https://github.com/codesenberg/bombardier).

### Results

| Name                          | Language      | Server          | Latency avg      | Requests      |
| ----------------------------  | ------------- | --------------- | ---------------- | ------------- |
| [static-rust](https://actix.rs/) | Rust | Actix Web | 1.35ms | 74kps |
| [graphql-crystal](https://github.com/graphql-crystal/graphql) | Crystal | Kemal | 3.00ms | 33kps |
| [gqlgen](https://github.com/99designs/gqlgen) | Go | net/http | 3.51ms | 28kps |
| [Juniper](https://github.com/graphql-rust/juniper) | Rust | Actix Web | 4.02ms | 25kps |
| [async-graphql](https://github.com/async-graphql/async-graphql) | Rust | Actix Web | 4.29ms | 23kps |
| [Hot Chocolate](https://github.com/ChilliCream/hotchocolate) | C# | ASP.NET | 6.38ms | 16kps |
| [agoo](https://github.com/ohler55/agoo) | Ruby/C | agoo | 7.42ms | 13kps |
| [Mercurius](https://github.com/mercurius-js/mercurius) | Node.js | Fastify | 7.80ms | 13kps |
| [graphql-go](https://github.com/graphql-go/graphql) | Go | net/http | 9.87ms | 10kps |
| [Hono](https://github.com/honojs/graphql-server) | Bun | HonoJS | 13.15ms | 7.6kps |
| [graphql-yoga](https://github.com/dotansimha/graphql-yoga) | Node.js | http | 14.35ms | 7.0kps |
| [Absinthe](https://github.com/absinthe-graphql/absinthe) | Elixir | Phoenix | 21.51ms | 4.6kps |
| [graphql-jit](https://github.com/zalando-incubator/graphql-jit) | Node.js | http | 21.77ms | 4.6kps |
| [apollo](https://github.com/apollographql/apollo-server) | Node.js | Express | 31.49ms | 3.2kps |
| [graphql-ruby](https://github.com/rmosolgo/graphql-ruby) | Ruby | Puma | 44.94ms | 2.9kps |
| [graphql-js](https://github.com/graphql/graphql-js) | Node.js | http | 40.31ms | 2.5kps |
| [Graphene](https://github.com/graphql-python/graphene) | Python | gunicorn | 97.97ms | 1.0kps |
| [Strawberry](https://github.com/strawberry-graphql/strawberry) | Python | gunicorn | 98.77ms | 1.0kps |
| [Sangria](https://github.com/sangria-graphql/sangria) | Scala | Akka HTTP | 131.58ms | 750ps |
