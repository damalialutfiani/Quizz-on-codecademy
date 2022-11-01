Lesson 8 – **Using Dictionaries**

1.    What will the following code output?

            combo_meals = {1: ["hamburger", "fries"], 2: ["hamburger", "fries", "soda"], 4: ["veggie burger", "salad", "soda"], 6: ["hot dog", "apple slices", "orange juice"]}
        
            print(combo_meals.get(3, ["hamburger", "fries"]))

      a.      KeyError
      
      b.      ["hot dog", "apple slices", "orange juice"]
      
      c.      **["hamburger", "fries"]**
      
      d.      ["veggie burger", "salad", "soda"]

2.    What does the following code output?

            inventory = {"iron spear": 12, "invisible knife": 30, "needle of ambition": 10, "stone glove": 20, "the peacemaker": 65, "demonslayer": 50}

            print(12 in inventory)

      a.    True
      
      b.	"iron spear"
      
      c.    KeyError

      d.	**False**

3.    What will the following code output?

            inventory = {"iron spear": 12, "invisible knife": 30, "needle of ambition": 10, "stone glove": 20, "the peacemaker": 65, "demonslayer": 50}

            print(inventory.get("stone glove", 30))

-	("stone glove", 20)
-	**20**
-	10
-	30
