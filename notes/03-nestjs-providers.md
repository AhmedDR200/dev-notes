# NestJS Providers Scope

By default NestJS providers are singletons shared across the whole app. Use `@Injectable({ scope: Scope.REQUEST })` when a provider needs per-request state, but be aware it forces every consumer up the chain into request scope too.
