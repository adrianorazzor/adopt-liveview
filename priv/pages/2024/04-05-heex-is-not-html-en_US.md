%{
title: "HEEx is not HTML",
author: "Lubien",
tags: ~w(getting-started),
section: "HEEx",
description: "What the heck is HEEx?"
}

---

Let me tell you a secret. Until now I kept calling the result of the HTML render function. The story isn't quite like that! `sigil_H` actually returns a data structure called HEEx. This structure is optimized to know when something has been modified based on its assigns and send the minimum amount of data from the client to the server.

%{
title: "How to pronounce HEEx?",
description: ~H"""
The creator's official pronunciation is "hiccs" as can be seen
<.link navigate="https://www.youtube.com/watch?v=FADQAnq0RpA&t=1420s" target="\_blank">in this video</.link> which introduces the structure.
"""
} %% .callout

In the next classes we will learn a little more about HEEx's super powers. In fact, you've already learned at least one: `assigns` are part of HEEx's range of functionalities.