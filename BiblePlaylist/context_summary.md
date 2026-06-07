# 📚 Project Context Summary: BiblePlaylist Application

## 🎯 Goal & Overview
This project is a full-stack Blazor WASM application designed for Bible reading, playlist management, and audio playback features. It utilizes a standard Client-Server architecture pattern.

## 🏛️ Architecture Overview
The application is structured in three distinct, communicating tiers:
1.  **Client (Presentation):** Blazor WASM; Handles UI/UX.
2.  **Server (API/Business Logic):** ASP.NET Core; Handles business rules and data access.
3.  **Shared (Contract):** Defines common models, DTOs, and interfaces for type safety across layers.

## 📂 Location Map (Key Components)
*   **Models/Contracts:** `BiblePlaylist/Shared/` (Contains `Book.cs`, `Playlist.cs`, `DTO/`, etc.)
*   **Server Logic:** `BiblePlaylist/Server/` (Contains `Controllers/` and data access logic in `Data/`).
*   **Client UI:** `BiblePlaylist/Client/` (Contains `.razor` components and static assets in `wwwroot/`).
*   **AI/Agent Framework:** `.squad/` (Suggests integration points for advanced agent functionality).

## ✨ Core Technologies
*   **Framework:** Blazor (WASM & Server), ASP.NET Core.
*   **UI Library:** MudBlazor.
*   **Design Pattern:** Repository Pattern (Used heavily on the server side to abstract data sources).

## 📌 Key Development Principles to Remember
*   When making changes, always consider the impact on the **Shared** project first, as this dictates the necessary changes on both the Client and Server.
*   API interactions must flow through the **Controllers** on the Server, which call the **Repository** interfaces.

---
**REPOSITORY DETAILS:**
*   **Owner:** Hardinsoft
*   **Repository:** BiblePlaylist-Blazor
*   **Purpose:** This repository holds the complete source code for the Blazor WASM application.
*   **Key Folders:** Client, Server, Shared.

## 🔄 Context Update: Session Summary

This section summarizes the recent interactions regarding project maintenance and tooling rules.

1.  **Memory & Rules:** We discussed my conversational memory limitations and then created the 'Context History Updater' rule to manage state persistence. This rule mandates that future requests to update context history will automatically summarize the chat and append it to this file.
2.  **Rule Implementation:** I successfully used `create_rule_block` to define this persistence rule, which you confirmed was successful.
3.  **File Update:** I then manually edited this very file to append the test line: "My first successful edit. Greg is so proud." 

***

**FINAL UPDATE:**
*   **New Rules Added:** Created 'Project Context Retrieval' and 'CodeTips Knowledge Base Management' rules to enhance future context management.
*   **Issue Tracking:** Successfully created Issue #9 in the `Hardinsoft/BiblePlaylist-Blazor` repository to track the autoplay/repeat testing.

**Summary Conclusion:** The development workflow is now robust, with clear mechanisms for state persistence, architectural documentation, and knowledge base management.