`less`: The less command in linux allows for a user to search for a provided file path and show its contents page by page. This is useful as you may not want to load the entirety of the contents at once to view.

General Input:
`less ./travel_guides/berlitz2/Vallarta-History.txt`

Output: Image

Explanation: The contents of `./travel_guides/berlitz2/Vallarta-History.txt` are shown.

General Input:
`less ./travel_guides/berlitz1/WhatToItaly.txt`
Output: Image

Explanation: The contents of `./travel_guides/berlitz1/WhatToItaly.txt` are shown.

---
`-S`: This option makes it so that long lines (longer than the screen) are not wrapped to fit in the screen, and only load after pressing the right arrow. This could be useful when wanting to load even less of the file.

Input:
`less -S ./travel_guides/berlitz2/Vallarta-History.txt`

Output: Image

Explanation: The larger lines of the file are only visible after moving to the right.

Input:
`less -S ./travel_guides/berlitz1/WhatToItaly.txt`

Output: Image

Explanation: Because the file had no lines that needed to be wrapped, the contents are displayed the same as without `-S`.

---
`-K`: This option allows you to use interrupt characters, like `ctrl C`, to exit the contents instead of just `:q`. This could be useful when you want to do less with a file/ only read and exit.

Input:
`less -K ./travel_guides/berlitz2/Vallarta-History.txt`

Output/ Explanation: While exiting the contents of the file, I was able to use `ctrl C`.

Input:
`less -K ./travel_guides/berlitz1/WhatToItaly.txt`

Output/ Explanation: While exiting the contents of the file, I was able to use `ctrl C`.

---
`-e`: This option exits the contents after reaching the end of the file a second time. This is useful for if you want to read a file and exit fairly quickly without spending more time with. 

Input:
`less -e ./travel_guides/berlitz2/Vallarta-History.txt`

Output: Image

Explanation: Upon reaching the end a second time, the contents were exited automatically.

Input:
`less -e ./travel_guides/berlitz1/WhatToItaly.txt`

Output: Image

Explanation: Upon reaching the end a second time, the contents were exited automatically.

---
`-E`: Similarly to `-e`, this option automatically exits the contents after reaching the end the first time. This is useful if you want to be fast and are certain you just want to read the contents once over. 

Input:
`less -E ./travel_guides/berlitz2/Vallarta-History.txt`

Output: Image

Explanation: Upon reaching the end, the contents were exited automatically.

Input:
`less -E ./travel_guides/berlitz1/WhatToItaly.txt`

Output: Image

Explanation: Upon reaching the end, the contents were exited automatically.
