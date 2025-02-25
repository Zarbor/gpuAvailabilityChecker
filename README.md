# GPU Availability Checker

This project is a Node.js application that checks the availability of specific GPU models from the NVIDIA store and sends notifications to a Discord channel when they are in stock.

## Features

- Checks the availability of NVIDIA GPU models (5090, 5080, 5070T, 5070).
- Sends notifications to a Discord channel using a webhook.
- Scheduled to run every minute using `node-cron`.

## Prerequisites

- Node.js (version 14 or later)
- npm (Node Package Manager)

## Installation

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd gpuAvailabilityChecker
    ```

2. Install the dependencies:
    ```sh
    npm install
    ```

3. Create a `.env` file in the root directory and add your Discord webhook URL and user IDs:
    ```env
    DISCORD_WEBHOOK_URL=your_discord_webhook_url
    USER_ID_1=your_user_id_1
    USER_ID_2=your_user_id_2
    ```

## Usage

To start the GPU availability checker, run the following command:
```sh
npm start