# Create Token - Solana Token Creation Program

This project is a Solana program built with Anchor framework that allows users to create new tokens on the Solana blockchain with metadata support.

## Features

- Create new token mints on Solana
- Configure token metadata (name, symbol, URI)
- Support for custom token decimals
- Integration with Metaplex Token Metadata Program

## Prerequisites

- Rust (latest stable version)
- Node.js and Yarn
- Solana CLI tools
- Anchor Framework

## Project Structure

```
.
├── app/                    # Frontend application (if any)
├── programs/              # Solana program source code
│   └── create-token/     # Main program
├── tests/                # Test files
├── migrations/           # Database migrations
└── Anchor.toml          # Anchor configuration
```

## Setup

1. Install dependencies:
```bash
yarn install
```

2. Build the program:
```bash
anchor build
```

3. Deploy the program:
```bash
anchor deploy
```

## Program Details

The main program provides the following functionality:

### Create Token Mint

Creates a new token mint with associated metadata.

Parameters:
- `token_decimals`: Number of decimal places for the token
- `token_name`: Name of the token
- `token_symbol`: Symbol of the token
- `token_uri`: URI pointing to the token's metadata

## Development

### Testing

Run the test suite:
```bash
anchor test
```

### Linting

Format code:
```bash
yarn lint:fix
```

Check code formatting:
```bash
yarn lint
```

## Dependencies

- @coral-xyz/anchor: ^0.31.1
- anchor-spl: For SPL token and metadata functionality
- TypeScript and related development tools

## License

ISC

## Security

This program has been built with security in mind, including:
- Proper PDA validation
- Authority checks
- Safe account initialization

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request 