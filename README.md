# Mermaid to Excalidraw Converter 🐻📊

_Transform diagrams with bear-like precision and intelligent conversion_ 🧉

[![Obsidian Plugin](https://img.shields.io/badge/Obsidian-Plugin-purple.svg)](https://obsidian.md/)
[![TypeScript](https://img.shields.io/badge/TypeScript-4.7.4-blue.svg)](https://www.typescriptlang.org/)
[![Mermaid](https://img.shields.io/badge/Mermaid-10.9.0-pink.svg)](https://mermaid.js.org/)
[![Excalidraw](https://img.shields.io/badge/Excalidraw-0.17.1-orange.svg)](https://excalidraw.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A powerful Obsidian plugin that seamlessly converts Mermaid.js diagram code blocks into fully functional Excalidraw drawings with proper text labels, intelligent formatting, and comprehensive diagram support.

---

## ✨ Intelligent Features

### 📊 **Complete Diagram Conversion**
- **Universal Mermaid Support** - Convert any Mermaid diagram type to Excalidraw format
- **Text Preservation** - Labels, annotations, and formatting maintained during conversion
- **Smart Rendering** - Automatic optimization for different diagram complexities
- **Bulk Processing** - Convert multiple diagrams simultaneously with one click

### 🎨 **Advanced Visual Processing**
- **Intelligent Shape Recognition** - Converts Mermaid elements to appropriate Excalidraw shapes
- **Layout Optimization** - Maintains spatial relationships and visual hierarchy
- **Style Preservation** - Colors, fonts, and formatting carried over accurately
- **Compression Technology** - LZ-string compression for optimal file compatibility

### ⚡ **Seamless Integration**
- **Native Obsidian Experience** - Ribbon icons and command palette integration
- **Excalidraw Plugin Compatibility** - Perfect integration with official Excalidraw plugin
- **File Format Standards** - Creates proper `.excalidraw.md` files with full compatibility
- **Workflow Optimization** - Single-click conversion from code to visual diagram

### 🔄 **Batch Operations**
- **Multi-Diagram Files** - Process entire documents with multiple Mermaid blocks
- **Automatic Numbering** - Generated files with intelligent naming conventions
- **Progress Feedback** - Real-time conversion status and success notifications
- **Error Recovery** - Graceful handling of malformed diagrams with detailed feedback

---

## 🧉 **Technology Stack**

**Core Framework**
- **Obsidian API** - Latest plugin architecture with modern TypeScript patterns
- **TypeScript 4.7.4** - Type-safe development with comprehensive interfaces
- **ESBuild 0.17.3** - Lightning-fast bundling with production optimizations

**Diagram Processing**
- **Mermaid 10.9.0** - Latest Mermaid.js engine with full syntax support
- **Excalidraw 0.17.1** - Advanced drawing library with shape primitives
- **Markdown-to-Text 0.1.2** - Text extraction and processing utilities
- **NanoID 4.0.2** - Unique identifier generation for diagram elements

**Data Management**
- **LZ-String 1.5.0** - Efficient compression for Excalidraw file format
- **JSON Processing** - Advanced object serialization and deserialization
- **File System Integration** - Native Obsidian vault file operations

**Development & Testing**
- **Jest 29.7.0** - Comprehensive testing framework with TypeScript support
- **TS-Jest 29.1.0** - TypeScript testing integration
- **ESLint 5.29.0** - Code quality and consistency enforcement

---

## 🚀 Installation Methods

### **Method 1: Manual Installation (Recommended)**

1. **Download Plugin Files**
   ```bash
   # Clone and build from source
   git clone https://github.com/YahyaZekry/obsidian-mermaid-to-excalidraw.git
   cd obsidian-mermaid-to-excalidraw
   npm install && npm run build
   ```

2. **Install in Obsidian**
   ```
   📁 Your-Vault/.obsidian/plugins/mermaid-to-excalidraw/
   ├── main.js (generated from build)
   ├── manifest.json
   └── styles.css (if applicable)
   ```

3. **Enable Plugin**
   - Open Obsidian Settings → Community Plugins
   - Disable "Restricted mode" if enabled
   - Find "Mermaid to Excalidraw Converter" and enable

### **Method 2: BRAT Installation (Beta)**

1. **Install BRAT Plugin** from Obsidian Community Plugins
2. **Add Repository** URL in BRAT settings: `YahyaZekry/obsidian-mermaid-to-excalidraw`
3. **Auto-Updates** - Plugin updates automatically through BRAT

---

## 🎯 **Usage Guide**

### **Single Diagram Conversion**

1. **Create Mermaid Diagram**
   ```mermaid
   graph TD
       A[🐻 Start Process] --> B{Decision Point}
       B -->|Yes| C[✅ Execute Action]
       B -->|No| D[❌ Alternative Path]
       C --> E[🎯 Success]
       D --> E
   ```

2. **Convert to Excalidraw**
   - Select entire Mermaid code block
   - Command Palette (Ctrl/Cmd + P) → "Convert Mermaid to New Excalidraw File"
   - New file created: `Converted-Mermaid-[timestamp].excalidraw.md`

3. **View Result**
   - Open generated file and switch to Excalidraw view
   - Full visual diagram with preserved labels and styling

### **Bulk Conversion Workflow**

1. **Multi-Diagram Document**
   ```markdown
   # My Diagrams
   
   ## Process Flow
   ```mermaid
   graph LR
       A --> B --> C
   ```
   
   ## System Architecture
   ```mermaid
   graph TD
       API --> DB
       DB --> Cache
   ```
   ```

2. **Batch Convert**
   - Click 🔄 ribbon icon or use "Convert All Mermaid Diagrams in File"
   - Generated files: `Filename-Diagram-1.excalidraw.md`, `Filename-Diagram-2.excalidraw.md`
   - Success notification with conversion count

---

## 📊 **Supported Diagram Matrix**

| Diagram Type | Support Level | Rendering Method | Text Labels | Notes |
|--------------|---------------|------------------|-------------|---------|
| **Flowcharts** | ✅ Excellent | Individual shapes | ✅ Full | Perfect shape and label conversion |
| **Sequence Diagrams** | ⚠️ Good | Individual shapes | ✅ Partial | Basic structure, some styling limitations |
| **Gantt Charts** | ✅ Excellent | Single image | ✅ Full | Complete timeline visualization |
| **State Diagrams** | ✅ Excellent | Single image | ✅ Full | All state transitions preserved |
| **ER Diagrams** | ✅ Excellent | Single image | ✅ Full | Database relationships maintained |
| **Pie Charts** | ✅ Excellent | Single image | ✅ Full | Data visualization with percentages |
| **Journey Maps** | ✅ Excellent | Single image | ✅ Full | User experience flows complete |
| **Requirement Diagrams** | ✅ Excellent | Single image | ✅ Full | System requirements preserved |
| **Timelines** | ✅ Excellent | Single image | ✅ Full | Chronological events with dates |
| **Mindmaps** | ✅ Excellent | Single image | ✅ Full | Hierarchical structures maintained |
| **Class Diagrams** | ⚠️ Basic | Individual shapes | ❌ Limited | Structure only, text needs improvement |
| **Git Graphs** | 🔄 Beta | Varies | ⚠️ Partial | Experimental support, results vary |

---

## 🔧 **Advanced Configuration**

### **Plugin Settings**
- **Output Directory** - Specify where converted files are saved
- **Naming Convention** - Customize generated file naming patterns
- **Compression Level** - Adjust LZ-string compression settings
- **Error Handling** - Configure behavior for malformed diagrams

### **Conversion Options**
- **Preserve Colors** - Maintain Mermaid color schemes in Excalidraw
- **Scale Factor** - Adjust diagram size during conversion
- **Text Rendering** - Choose between shape labels or floating text
- **Background Style** - Set transparent or solid backgrounds

---

## 🛠️ **Development**

### **Building the Plugin**

```bash
# Install dependencies
npm install

# Development build with watch mode
npm run dev

# Production build
npm run build

# Run test suite
npm test

# Type checking
npx tsc --noEmit --skipLibCheck
```

### **Testing Framework**

```bash
# Run all tests
npm test

# Watch mode for development
npm test -- --watch

# Coverage report
npm test -- --coverage
```

### **Contributing**
1. Fork the repository
2. Create feature branch (`git checkout -b feature/bear-diagram-power`)
3. Add comprehensive tests for new diagram types
4. Ensure TypeScript type safety
5. Commit with descriptive messages (`git commit -m '🐻 Add bear-strength conversion features'`)
6. Open Pull Request with test coverage

---

## 🏗️ **Architecture Overview**

```
obsidian-mermaid-to-excalidraw/
├── src/
│   ├── main.ts                    # Plugin entry point and Obsidian API
│   ├── MermaidConverter.ts        # Core conversion logic
│   ├── ExcalidrawGenerator.ts     # Excalidraw format generation
│   ├── DiagramProcessor.ts        # Mermaid parsing and analysis
│   ├── FileManager.ts            # Obsidian file operations
│   └── utils/
│       ├── compression.ts        # LZ-string utilities
│       ├── shapes.ts            # Excalidraw shape generation
│       └── types.ts             # TypeScript definitions
├── __tests__/                    # Jest test suite
│   ├── converter.test.ts        # Conversion logic tests
│   ├── diagrams.test.ts         # Diagram type tests
│   └── integration.test.ts      # End-to-end tests
├── manifest.json                 # Obsidian plugin manifest
├── esbuild.config.mjs           # Build configuration
└── package.json                 # Dependencies and scripts
```

---

## 🤝 **Compatibility & Requirements**

### **Plugin Dependencies**
- **✅ Excalidraw Plugin** - Official Obsidian Excalidraw plugin required for viewing
- **✅ Obsidian 0.15.0+** - Modern Obsidian version with plugin API support
- **✅ Cross-Platform** - Works on Windows, macOS, and Linux

### **Supported Formats**
- **Input** - Standard Mermaid code blocks with ```mermaid syntax
- **Output** - Compressed `.excalidraw.md` files with full compatibility
- **Integration** - Seamless workflow with existing Mermaid and Excalidraw content

---

## 🏆 **Acknowledgments**

### **Based on Excalidraw's Work**
This plugin utilizes and extends the core functionality of [`@excalidraw/mermaid-to-excalidraw`](https://github.com/excalidraw/mermaid-to-excalidraw) library.

**Original License**: MIT License, Copyright (c) 2023 Excalidraw

### **Technology Credits**
- **Mermaid.js Team** - Excellent diagram syntax and rendering engine
- **Excalidraw Team** - Beautiful drawing library and conversion tools
- **Obsidian Team** - Powerful plugin architecture and community support

---

## 📄 **License**

MIT License - see [LICENSE](LICENSE) file for complete details.

**Copyright (c) 2025 The Bear Code**

*This plugin extends the MIT-licensed `@excalidraw/mermaid-to-excalidraw` library*

---

## 🐻 **Author**

**Yahya Zekry** • The Bear Code  
- GitHub: [@YahyaZekry](https://github.com/YahyaZekry)  
- LinkedIn: [Professional Profile](https://www.linkedin.com/in/yahyazekry/)  
- Project: [Mermaid to Excalidraw Converter](https://github.com/YahyaZekry/obsidian-mermaid-to-excalidraw)

---

**Built with ❤️ for the Obsidian community • The Bear Code philosophy: Smart conversion, visual excellence 🐻📊**

<div align="center">
  <a href="https://buymeacoffee.com/YahyaZekry" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Support The Bear Code" height="45" />
  </a>
</div>

<div align="center">
  <sub>Converting diagrams with bear-like precision, one Mermaid at a time 🧉</sub>
</div>