# Smart Farm System

This is a Rust implementation of a Smart Farm System, designed to handle various aspects of smart farming, including tracking crops, tasks, expenses, and providing functionalities such as creating, updating, and querying crop-related information.

## Technologies Used

- **Rust**: The programming language used for the backend implementation.
- **Candid**: Used for defining the canister interface.
- **Internet Computer (IC)**: Utilizes IC-specific libraries (`ic_cdk`) for interactions with the Internet Computer.

## Components

### Data Structures
- **Crop**: Represents information about a crop, including its name, description, quantity, and timestamps.
- **Task**: Represents a task related to smart farming, including details like name, description, completion status, associated crop ID, and timestamps.
- **Expense**: Represents an expense entry, with fields for description, amount, and timestamp.

### Functionality
- **Smart Farm Management**: Create, update, and retrieve information about crops.
- **Task Management**: Create, update, complete, and delete tasks associated with smart farming.
- **Expense Management**: Create, update, and delete expense entries.
- **Budget Calculation**: Calculates the budget by considering total expenses and the value of crops.
- **Crop Rotation Recommendations**: Provides recommendations for crop rotation based on the input crop.

## Local Deployment

To deploy this Smart Farm System on a local machine, follow these steps:

1. **Install Rust**: Ensure that Rust is installed on your machine. You can install it from [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install).

2. **Clone the Repository**: Clone this repository to your local machine.

    ```bash
    git clone https://github.com/ogola5/smart_farm.git
    ```

3. **Build the Project**: Navigate to the project directory and build the project.

    ```bash
    cd smart_farm
    cargo build
    ```

4. **Run the Project Locally**: Run the project locally using the following command.

    ```bash
    cargo run
    ```

5. **Access the Endpoints**: Once the project is running, you can access the provided endpoints for interacting with the Smart Farm System.

## Canister Deployment

To deploy this Smart Farm System on the Internet Computer, you need to follow the steps outlined in the Internet Computer documentation. Here is a simplified overview:

1. **Internet Computer SDK**: Install the DFINITY Canister SDK by following the instructions at [https://sdk.dfinity.org/docs/download.html](https://sdk.dfinity.org/docs/download.html).

2. **Start the Canister**: Build the canister using the following command:

    ```bash
    dfx start
    ```

3. **Deploy the Canister**: Deploy the canister to the Internet Computer.

    ```bash
    dfx deploy
    ```

4. **Interact with the Canister**: Once deployed, you can interact with the canister using the generated canister ID.

    ```bash
    dfx canister call <canister-id> <function-name>
    ```
