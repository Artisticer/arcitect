# arcitect
arh disign
import matplotlib.pyplot as plt
import matplotlib.patches as patches

# Create a figure and axis
fig, ax = plt.subplots()

# Add a rectangular room to the floor plan
room = patches.Rectangle((1, 1), 5, 8, linewidth=1, edgecolor='r', facecolor='none')
ax.add_patch(room)

# Add a door to the room
door = patches.Rectangle((2, 1), 1, 0.1, linewidth=1, edgecolor='b', facecolor='b')
ax.add_patch(door)

# Add a window to the room
window = patches.Rectangle((4, 1), 1, 1, linewidth=1, edgecolor='g', facecolor='g')
ax.add_patch(window)

# Set axis limits
ax.set_xlim(0, 8)
ax.set_ylim(0, 10)

# Set axis labels
ax.set_xlabel('Length (m)')
ax.set_ylabel('Width (m)')

# Add a title
ax.set_title('Simple Floor Plan')

# Display the floor plan
plt.show()
