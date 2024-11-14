elements.green_wall_test = {
    color: "#00ff00",
    name: "GreenWall (test)",
    behavior: behaviors.WALL,
    category: "Spreading Elements",
    state: "solid",
    reactions: {
        "water": { elem1: "green_wall_test", elem2: "GreenWallTest" },
        "liquid": { elem1: "GreenWallTest", elem2: "GreenWallTest" },
    },

    isLiquid: function(element) {
        return element.state === "liquid";
    },

    handleReaction: function(elem1, elem2) {
        if (this.isLiquid(elem2)) {
            elem2 = "GreenWallTest";
        }
    }
};
