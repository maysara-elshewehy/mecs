# ╠═ MECS ═╣

MECS is a simple and unified way to write code and create projects in a way that makes programming more fun and organized. Let's get started . . 🚀

- ## 📚 Introduction

    **MECS** stands for **`M`** methodologies, **`E`** examples, **`C`** coding styles, and **`S`** standards. With **`MECS`**, you can efficiently organize your projects, save time, and maintain a consistent context across all your projects.


    | INDEX                   | DESC                         |
    | ----------------------- | ---------------------------- |
    | [Project](#project)     | a way to develop a project ! |
    | [Scripting](#scripting) | a way to scripting !         |
    | [Templates](#templates) | a way to start anything !    |

---

- ### Project

    1. The `/root` directory should be the main project directory.

    2. `/root` must contain a `src` folder, which houses the actual code and related components.

        > like **Documents** in `/src/docs`, **Unit Tests** in `/src/tests` and **Source code** in `src/code`

        - #### Main file
            The main script should be located in `/src/code/main.?`.

        - #### Modules
            Additional modules should be placed in `/src/code/modules/?.?`.

- ### Scripting

    1. Each script must start with an introductory comment, as shown below:

        ```ts
        /**
        * @name                                    main.ts                          (*) Required
        * @description                             the main file (entry point)      (*) Required
        * @author                                  Maysara Elshewhy                 (!) Optionally
        * @repo                                    https://github.com/?             (!) Optionally
        * @package                                 https://npmjs.com/?              (!) Optionally
        * ..
        */
        ```

    2. Scripts should be divided into several sections:

       - **PACK** for imports:

            ```ts
            /* ---------------------------------------- PACK ----------------------------------------  */

                import { someFunction }                 from 'somePackage';

            /* ---------------------------------------- ---- ----------------------------------------  */
            ```

       - **INIT** for constants and initializations:

            ```ts
            /* ---------------------------------------- INIT ----------------------------------------  */

                const someString    : string            = 'Maysara';

            /* ---------------------------------------- ---- ----------------------------------------  */
            ```

       - **CORE** for the main code of the script:

            ```ts
            /* ---------------------------------------- CORE ----------------------------------------  */

                /**
                     * ?
                    *
                    * @param {string} input             - ?
                    *
                    *
                    * @return {string} ?
                */
                export const myFunction
                = (input: string)
                : string =>
                {
                    return Helpers.DoIT(input);
                    return 'Hello ' + input;
                }

            /* ---------------------------------------- ---- ----------------------------------------  */
            ```

       - **HELP** for helper functions:

            ```ts
            /* ---------------------------------------- CORE ----------------------------------------  */

                const Helpers =
                {
                    DoIT: (input: string)
                    : string =>
                    {
                        return 'Hello ' + input;
                    },
                }

            /* ---------------------------------------- ---- ----------------------------------------  */
            ```

    3. to export something use `export ?` | `export { ? }` | `export * from '?'`


- ### Templates

    | TEMPLATE                                                                            | DESCRIPTION                                                                                      |
    | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
    | [`MECS` npm package](https://github.com/Maysara-Elshewehy/mecs-npm-package)                | A ready `Node.js` project with `TypeScript` for publishing on `npm`                              |
    | [`MECS` electron app]([?](https://github.com/Maysara-Elshewehy/mecs-electron-app)) | A ready `Node.js` project with `JavaScript` and `@je-es` framework to quickly build desktop apps |

---

> **MECS** == **M**aysara **E**lshewehy **C**ode **S**tyle !

> **Made with ❤ by [Maysara Elshewehy](https://github.com/Maysara-Elshewehy)**