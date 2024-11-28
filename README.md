
# Enterprise Ethereum Analysis Agent


[![Join our Discord](https://img.shields.io/badge/Discord-Join%20our%20server-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/agora-999382051935506503) [![Subscribe on YouTube](https://img.shields.io/badge/YouTube-Subscribe-red?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@kyegomez3242) [![Connect on LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kye-g-38759a207/) [![Follow on X.com](https://img.shields.io/badge/X.com-Follow-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/kyegomezb)


[![Swarms Framework](https://img.shields.io/badge/Built%20with-Swarms-blue)](https://github.com/kyegomez/swarms)


Real-time, AI-powered analysis of high-value Ethereum transactions using the Swarms framework.

[![GitHub stars](https://img.shields.io/github/stars/The-Swarm-Corporation/eth-agent)](https://github.com/The-Swarm-Corporation/eth-agent/stargazers)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Built with Swarms](https://img.shields.io/badge/built%20with-Swarms-orange.svg)](https://github.com/kyegomez/swarms)

## Overview

The Enterprise Ethereum Analysis Agent is a production-grade system that monitors and analyzes high-value Ethereum transactions in real-time. By combining Web3 technology with advanced AI capabilities through the Swarms framework, it provides institutional-grade insights into significant blockchain movements.

### Key Features

- **Real-time Transaction Monitoring**: Automated detection of transactions over 100 ETH
- **AI-Powered Analysis**: Instant, comprehensive analysis using GPT-4
- **Market Context Integration**: Real-time price data and USD value assessment
- **Enterprise-grade Logging**: Structured logging with rotation policies
- **Persistent Storage**: CSV-based transaction and analysis archival
- **Contract Interaction Detection**: Automatic identification of smart contract interactions
- **Event Tracking**: Comprehensive logging of contract events
- **Market Impact Assessment**: Real-time analysis of potential market effects

## Installation

### Prerequisites

- Python 3.9+
- OpenAI API key
- Internet connection for blockchain and price data access

### Setup

1. Clone the repository:
```bash
git clone https://github.com/The-Swarm-Corporation/eth-agent.git
cd eth-agent
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the project root:
```env
OPENAI_API_KEY=your_api_key_here
```

## Usage

Start the analysis system:

```bash
python eth_analyzer.py
```

The system will:
1. Begin monitoring the Ethereum blockchain
2. Detect transactions ≥ 100 ETH
3. Perform AI analysis of each transaction
4. Save results to `ethereum_analysis.csv`
5. Display real-time analysis in the console

### Configuration

Key parameters can be adjusted in `eth_analyzer.py`:

```python
analyzer = EthereumAnalyzer(
    min_value_eth=100.0,  # Minimum transaction value to track
)
```

### Output Format

The system generates two types of output:

1. Console Output (Real-time):
```
===========================================
New Transaction Analysis
Hash: 0x123...
Value: 150.00 ETH ($300,000.00)
Current ETH Price: $2,000.00
===========================================
[AI Analysis Output]
===========================================
```

2. CSV Output (Archived):
- timestamp
- transaction_hash
- from_address
- to_address
- value_eth
- value_usd
- eth_price
- gas_used
- gas_price_gwei
- block_number
- analysis

## System Architecture

The system operates through several integrated components:

1. **Blockchain Monitor**: Interfaces with Ethereum network
2. **Transaction Analyzer**: Processes and filters transactions
3. **AI Analysis Engine**: Generates insights via GPT-4
4. **Data Persistence**: Manages CSV storage
5. **Logging System**: Maintains operational logs

## Dependencies

- [Swarms](https://github.com/kyegomez/swarms): AI agent framework
- web3.py: Ethereum interaction
- loguru: Logging system
- requests: API interactions
- pandas: Data management
- python-dotenv: Environment management

## Enterprise Support

For enterprise deployment assistance or custom feature development, contact:
- Website: [swarms.ai](https://swarms.ai)
- Discord: [Join Swarms Community](https://swarms.ai)

## Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with [Swarms](https://github.com/kyegomez/swarms)
- Uses OpenAI's GPT-4 for analysis
- Ethereum blockchain community

## Security

Please report security issues directly to security@swarms.ai

---
Maintained by [The Swarm Corporation](https://github.com/The-Swarm-Corporation)
