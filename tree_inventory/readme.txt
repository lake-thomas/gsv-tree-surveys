# City Tree Inventories

The `tree_inventory/code` module provides scripts for processing city tree inventory datasets and reconciling inventory labels with model outputs from GSV imagery.

## Files

- **AutoArborist_Species_Level_Images**: Verify matching between tree genera and tree species based on city inventories.
- **inventory_autoarborist_merger**: attempts to match AutoArborist longitude/latitude pairs with city inventory coordinates.
- **inventory_name_appender**: creates cleaned genus/species naming fields for detected organisms.
