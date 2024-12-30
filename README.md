# My Personal Naming Convention 📜

> **Why❓**
>
> I simply work on libraries that contain hundreds of files with thousands of lines and hundreds of functions 😔, and because this has become my way of life, these are the rules I will follow when writing any code from now on **_(Damn the rules of the world that don't suit me 😶)_**.

- ## Rules

    - #### Sections

        > `padding = 2` _(1 line before content, 1 line after)_, `margin = 3` _(3 lines between sections)_

        ```zig
        // ╔══════════════════════════════════════ NAME ══════════════════════════════════════╗

            ...

        // ╚══════════════════════════════════════════════════════════════════════════════════╝
        ```

    - #### Sub-Sections

        > `padding = 2`, `margin = 2`

        ```zig
        // ┌──────────────────────────── NAME ────────────────────────────┐

            ...

        // └──────────────────────────────────────────────────────────────┘
        ```

    - #### Structures

        ```zig
        /// Desc.
        const MyStruct = struct {
            /// Desc.
            m_field,
            /// Desc.
            m_fieldTwo,
        };
        ```

    - #### Functions

        ```zig
        /// Desc.
        pub fn functionName(_argument, _argumentTwo) bool {
            var _Local;
            var _LocalVariable;

            if(..) |__res| {
                if(..) |___resTwo| {
                    ...
                }
            }

            return false;
        }
        ```
---

> Almost everyone has told me how ugly this style is, well it's like you've never seen anything this beautiful before, so it makes sense that it would be different _(bad)_ for you **But that doesn't mean it's bad for me**.
