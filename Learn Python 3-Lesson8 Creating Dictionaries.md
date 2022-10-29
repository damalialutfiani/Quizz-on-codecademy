Lesson 8 – **Creating Dictionaries**

1.  What will the following code output?

        conference_rooms = ["executive", "hopper", "lovelace", "pod", "snooze booth"]
        capacity = [7, 20, 6, 2, 1]
        room_dict = {key:value for key, value in zip(conference_rooms, capacity)}

        print(room_dict)

    a.	**{"executive": 7, "hopper": 20, "lovelace": 6, "pod": 2, "snooze booth": 1}**

    b.	[("executive", 7), ("hopper", 20), ("lovelace", 6), ("pod", 2), ("snooze booth", 1)}

    c.	{7: "executive", 20: "hopper", 6: "lovelace", 2: "pod", 1: "snooze booth": 1}

    d.	["executive", 7, "hopper", 20, "lovelace", 6, "pod", 2, "snooze booth", 1]

2.  What is the value of inventory after this code run?

        inventory = {"iron spear": 12, "invisible knife": 30, "needle of ambition": 10, "stone glove": 20}
            
        inventory["invisible knife"] = 40
        inventory["mithril shield"] = 25

    a.  **{"iron spear": 12, "invisible knife": 40, "needle of ambition": 10, "stone glove": 20, "mithril shield": 25}**

    b.  {"iron spear": 12, "invisible knife": 30, "needle of ambition": 10, "stone glove": 20, “invisible knife”: 40, "mithril shield": 25}

    c.  {"iron spear": 12, "invisible knife": 70, "needle of ambition": 10, "stone glove": 20}

    d.  {"iron spear": 12, "invisible knife": 70, "needle of ambition": 10, "stone glove": 20, "mithril shield": 25}

3.  What is the line of code to initialize an empty dictionary called thesaurus?

    a.  thesaurus = []

    b.	thesaurus = empty_dict()

    c.	thesaurus = new Dictionary()

    d.	**thesaurus = {}**

4.  Which of these is an invalid dictionary (will result in a TypeError when trying to run)?

    a.  **{["apple", "orange"]: "fruit", ["broccoli"]: "vegetable", ["salt", "paprika", "saffron"]: "spice"}**

    b.	{2: ["apple", "orange"], 1: ["broccoli"], 3: ["salt", "paprika", "saffron"]}
        
    c.  {"fruit": “apple”, "vegetable": 100, “spice”: ["salt", "paprika", "saffron"]}
        
    d.  All these are valid
