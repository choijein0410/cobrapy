# Release notes for cobrapy x.y.z

## New features

- Added `chrr` sampler for flux polytope sampling, which is guaranteed to yield uniformly distributed samples. Uses the optional dependency `hopsy`, installable with `pip install cobra[chrr]`.

## Fixes
- Rare race condition in cache directory creation from running seperate processes loading cobrapy on clean machine fixed. (https://github.com/opencobra/cobrapy/issues/1476)
- `find_blocked_reactions` now raises an explicit `OptimizationError` when the initial model optimization returns a non-optimal (e.g. infeasible) status, instead of silently proceeding with an invalid solution and potentially reporting false-positive blocked reactions. (https://github.com/opencobra/cobrapy/issues/838)


## Other

## Deprecated features


## Backwards incompatible changes
