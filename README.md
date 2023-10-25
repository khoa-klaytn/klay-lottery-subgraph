# Klay Lottery Subgraph

TheGraph exposes a GraphQL endpoint to query the events and entities within the Binance Smart Chain and Klay Lottery ecosystem.

Currently, there are multiple subgraphs, but additional subgraphs can be added to this repository, following the current architecture.

## Subgraphs

**[Lottery](https://thegraph.com/legacy-explorer/subgraph/klay-lottery/lottery)**: Tracks all Klay Lottery with rounds, draws and tickets.

## Deployment

For any of the subgraph: `blocks` as `[subgraph]`

1. Run the `cd subgraphs/[subgraph]` command to move to the subgraph directory.

2. Run the `pnpm codegen` command to prepare the TypeScript sources for the GraphQL (generated/\*).

3. Run the `pnpm build` command to build the subgraph, and check compilation errors before deploying.

4. Run `graph auth --product hosted-service '<ACCESS_TOKEN>'`

5. Deploy via `pnpm deploy`.
