# world_works
This is how to code for finding the Tile price of a given surface
# Find  the number of Tile to Cover the W x H Floor

room_width = int(input("What is the width of room: "))
room_height = int(input("What is the height of room: "))


def room_area():
    result = room_height * room_width
    return result


tile_dimensions = int(input("What is the side of tile: "))


def tile_area():
    result = tile_dimensions ** 2
    return result


final_result = int(room_area()) / int(tile_area())
print(str(final_result) + " is the number of tiles.")

# Find the Cost of Tile to Cover W x H Floor
cost_tile = int(input("What is the cost of each tile: "))
final_tile_cost = final_result * cost_tile
print(str(final_tile_cost) + " is the cost of tiles.")
