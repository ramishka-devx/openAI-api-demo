# OpenAI API Demo

A simple Node.js application demonstrating how to use the OpenAI API to generate AI-powered content, specifically showcasing haiku generation using GPT-4o-mini.

## Features

- 🤖 OpenAI GPT-4o-mini integration
- 📝 Haiku generation example
- 🔐 Environment variable configuration
- 🚀 Easy setup and deployment

## Prerequisites

Before running this application, make sure you have:

- Node.js (version 14 or higher)
- npm or yarn package manager
- An OpenAI API key

## Installation

1. Clone the repository:
   ```bash
   git clone <your-repository-url>
   cd openAI-api-demo
   ```

2. Navigate to the API directory:
   ```bash
   cd api
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Create a `.env` file in the `api` directory:
   ```bash
   touch .env
   ```

5. Add your OpenAI API key to the `.env` file:
   ```
   OPENAI_API_KEY=your_openai_api_key_here
   ```

## Usage

### Running the Application

1. Start the application:
   ```bash
   npm start
   ```

2. The application will execute and display a generated haiku about AI in the console.

### Example Output

```
{
  role: 'assistant',
  content: 'Silicon dreams wake,\nAlgorithms dance with thought—\nFuture whispers now.'
}
```

## Configuration

The application uses the following environment variables:

| Variable | Description | Required |
|----------|-------------|----------|
| `OPENAI_API_KEY` | Your OpenAI API key | Yes |

## Project Structure

```
openAI-api-demo/
├── api/
│   ├── index.js          # Main application file
│   ├── package.json      # Node.js dependencies and scripts
│   └── .env             # Environment variables (create this)
├── LICENSE
└── README.md
```

## API Details

The application uses:
- **Model**: `gpt-4o-mini`
- **Store**: `true` (for conversation storage)
- **Role**: User input requesting haiku generation

## Dependencies

- `openai` (^5.8.2) - Official OpenAI API client
- `dotenv` (^17.0.1) - Environment variable loader
- `nodemon` (^3.1.10) - Development tool for auto-restarting

## Getting Your OpenAI API Key

1. Visit [OpenAI's website](https://platform.openai.com/)
2. Sign up or log in to your account
3. Navigate to the API section
4. Generate a new API key
5. Copy the key and add it to your `.env` file

## Customization

You can modify the `index.js` file to:
- Change the AI model (e.g., `gpt-4`, `gpt-3.5-turbo`)
- Modify the prompt for different types of content
- Add error handling and response processing
- Implement different conversation flows

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## Troubleshooting

### Common Issues

1. **API Key Error**: Make sure your `.env` file is in the correct directory and contains a valid OpenAI API key.

2. **Module Not Found**: Ensure all dependencies are installed by running `npm install`.

3. **Permission Errors**: Check that you have proper permissions to read the `.env` file.

## Support

If you encounter any issues or have questions, please:
- Check the [OpenAI API documentation](https://platform.openai.com/docs/)
- Review the troubleshooting section above
- Open an issue in this repository

## Acknowledgments

- OpenAI for providing the powerful GPT models
- The Node.js community for excellent tooling and libraries

---

**Note**: Remember to keep your API key secure and never commit it to version control. Always use environment variables for sensitive information.
