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
