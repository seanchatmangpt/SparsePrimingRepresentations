# SPR — Negative-Overhead Abstraction

- An abstraction has negative overhead when using the abstraction is cheaper than bypassing it.
- The abstraction should remove duplicated decisions, boilerplate, invalid states, integration glue, or verification work.
- Runtime zero-cost is insufficient if cognitive, operational, migration, or proof cost rises.
- The strongest abstraction improves both local ergonomics and system-wide correctness.
- A good type can eliminate branches before runtime.
- A good generator can eliminate handwritten synchronization between equivalent projections.
- A good protocol can make the correct path shorter than the unsafe path.
- A good ontology can replace repeated translation with shared meaning.
- Abstraction debt appears when callers must understand hidden internals to use the abstraction correctly.
- Leakage is evidence that the abstraction boundary is incomplete or misplaced.
- Measure abstraction value across authoring cost, execution cost, verification cost, change amplification, and defect surface.
- The ideal abstraction compounds: each new consumer increases reuse while adding less marginal coordination cost.
