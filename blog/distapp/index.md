# DistApp

In today's digital era, web applications have become an integral part of businesses and organizations' daily operations. However, ensuring the safety and reliability of these applications remains a challenging task. To address this issue, a new software design idea has emerged - the frontend-based interconnected application system.

This system comprises a "master" application publicly accessible at a URL, which runs the engine app. The engine app is responsible for discovering and loading reliable scripts from external sources. Once fetched, the engine loads the contained applications and performs a security check to verify their reliability and accessibility via a public URL.

The engine app operates in two modes: stable and sandbox mode. In stable mode, the engine ensures that the loaded application does not contain any code flagged as a security risk. In sandbox mode, the engine restricts the application's access to the underlying system and isolates it from other applications running on the system.

To maintain the application's integrity, the engine app performs a certificate check to confirm the loaded application's trustworthiness. This process guarantees that the user trusts the file hosted at the URL and ensures that the application is safe for use.

One of the significant advantages of this system is its ability to facilitate the deployment of safe and reliable web applications without the need for extensive security checks or code audits. This feature allows organizations to focus on developing valuable applications for their customers without sacrificing security and reliability.

In conclusion, the frontend-based interconnected application system offers a new and innovative approach to building safe and reliable web applications. Through the engine app's functionality, businesses and organizations can easily and quickly deploy applications while maintaining their security and reliability. The system's flexibility and effectiveness make it an ideal solution for organizations looking to build high-quality web applications.

