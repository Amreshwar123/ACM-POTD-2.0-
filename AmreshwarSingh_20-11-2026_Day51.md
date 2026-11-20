def count_picked_leaves(leaves):
    """
    Count how many leaves Alyona picks from an iterable of leaves.

    Each item in `leaves` can be a (color, species) tuple/list
    or a dictionary with 'color' and 'species' keys.
    """
    picked = set()

    for leaf in leaves:
        if isinstance(leaf, dict):
            key = (leaf["color"], leaf["species"])
        else:
            key = (leaf[0], leaf[1])

        if key not in picked:
            picked.add(key)

    return len(picked)


# Example usage
fallen_leaves = [
    ("red", "maple"),
    ("yellow", "birch"),
    ("red", "maple"),   # Same color & species as first leaf -> skipped
    ("brown", "maple"),  # Different color, same species -> picked
    ("red", "oak"),      # Same color, different species -> picked
]

print("Leaves picked:", count_picked_leaves(fallen_leaves))  
