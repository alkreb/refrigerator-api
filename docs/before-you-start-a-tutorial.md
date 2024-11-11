# Before you start a tutorial

These are the steps you must do before you can run
the tutorials for the **Refrigerator API**.

Expect this preparation to take about 20 minutes to complete.

## Preparing for the tutorials

To complete the tutorials in this section, you need the following.
You might want to open the links in separate brower tabs before you start installing the software.

* A [GitHub account](https://github.com)
* A development system (PC, Mac, or Linux) running a current or
long-term support (LTS version of the operating system).
* The following software on your development system:
    * [Git](https://docs.github.com/en/get-started/quickstart/set-up-git) (for the command line)
    * [GitHub Desktop](https://desktop.github.com) (optional)
    * A fork of the [Refrigerator API repo](https://github.com/neverett/refrigerator-api)
    * A current/LTS version of `node.js`
    * A current version of [json-server](https://www.npmjs.com/package/json-server)
    * A current copy of the database file. You can get this by syncing your fork.
    * **TIP**: If you're using a fork of the repo, create a working branch in which to do your tutorials. Create a new branch for each tutorial to prevent a mistake in one from affecting your work in another.
    * The [Postman desktop app](https://www.postman.com/downloads/). Because you run the **Refrigerator API** on your development system with an `http://localhost` hostname, the web version of Postman can't perform the exercises.

## Test your development system

To test your development system:

1. Create and checkout a test branch of your fork of the Refrigerator API repo. Your `GitHub repo workspace` is the directory that contains your fork of the `refrigerator-api` repo.

    ```shell
    cd <your GitHub repo workspace>
    ls
    # (see the refrigerator-api directory in the list)
    cd refrigerator-api
    git checkout -b tutorial-test
    cd api
    json-server -w refrigerator-api-source.json
    ```

    If your development system is installed correctly, you should see
    the service start and display the URL of the service: `http://localhost:3000`.

2. Make a test call to the service.

    ```shell
    curl http://localhost:3000/fridge
    ```

3. If the service is running correctly, you should see a list of fridge items from the service, such as in this example.

    ```js
        [
            {
                "category": "dairy",
                "type": "cheese",
                "subtype": "deli sliced pepper jack",
                "description": "",
                "sell_by_date": "NA",
                "best_by_date": "12/28/2024",
                "purchase_date": "07/01/2024",
                "fridge_section": "middle shelf",
                "id": 1
            },
            {
                "category": "dairy",
                "type": "milk",
                "subtype": "2%",
                "description": "",
                "sell_by_date": "NA",
                "best_by_date": "12/28/2024",
                "purchase_date": "12/15/2024",
                "fridge_section": "top shelf",
                "id": 2
            },
            {
                "category": "condiments",
                "type": "salad dressing",
                "subtype": "",
                "description": "Ginger Dressing",
                "sell_by_date": "2/27/2025",
                "best_by_date": "",
                "purchase_date": "07/01/2024",
                "fridge_section": "door top shelf",
                "id": 3
            },
            {
                "category": "leftovers",
                "type": "lasagna",
                "subtype": "",
                "description": "",
                "Refrigeration_date": "12/14/2024",
                "best_by_date": "12/17/2024",
                "purchase_date": "NA",
                "fridge_section": "middle shelf",
                "id": 4
            }
        ]
    ```

If you don't see the list of items, or receive an error in any step
of the procedure, investigate and correct the error before continuing.
Some common situations that cause errors include:

1. You mistyped a command.
2. You aren't in the correct directory.
3. A required software component didn't install correctly.
4. A required software component isn't up to date.

If you see the list of items from the API, you're ready to do
the [Tutorials](tutorials/index.md).
