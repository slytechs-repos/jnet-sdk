![Sonatype Nexus (Snapshots)](https://img.shields.io/nexus/s/com.slytechs.jnet/jnet-sdk-parent?server=https%3A%2F%2Fs01.oss.sonatype.org%2F)

# jnet-sdk

jnet-sdk is a Maven aggregator project that combines all jNet projects into a single build. This project simplifies the build process and dependency management for the jNet ecosystem.

## Included Projects

This aggregator includes the following jNet projects:

- jNet Runtime
- PCAP
- Protocols
- jNetWorks
- DPDK
- Napatech NTAPI

## Prerequisites

Before building this project, ensure you have the following installed:

- Java Development Kit (JDK) 22 or higher
- Maven 3.6.0 or higher

## Building the Project

To build all the included projects, run the following command in the root directory of this repository:

```bash
mvn clean install
```
or with publishing permission:
```bash
mvn clean deploy
```

## Project Structure
The project structure is as follows:

```
jnet-sdk/
├── pom.xml
├── jnetruntime-sdk/
├── jnetpcap-sdk/
├── protocol-pack-sdk/
├── jnetworks-sdk/
├── jnetdpdk-sdk/
└── jnetntapi-sdk/
```

> **Note:** Each SDK has a corresponding github repo and git sub-project as well asone or more maven modules. Remember to clone with the "recursive" option on, to also clone the modules inside.

## Usage
To use the jnet-sdk in your project, add the following dependency to your pom.xml:

![Sonatype Nexus (Snapshots)](https://img.shields.io/nexus/s/com.slytechs.jnet/jnet-sdk-parent?server=https%3A%2F%2Fs01.oss.sonatype.org%2F)

```xml
<dependency>
    <groupId>com.jnet</groupId>
    <artifactId>jnet-sdk</artifactId>
    <version>X.Y.Z</version>
    <type>pom</type>
</dependency>
```
## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
Sly Technologies Free License

See: http://www.slytechs.com/free-license-text

## Contact
Sly Technologies: sales@slytechs.com

Visit: http://slytechs.com


