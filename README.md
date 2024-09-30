    // VIM Config
    "vim.statusBarColors.easymotioninputmode": "#ca08b0",
    "vim.statusBarColors.easymotionmode": "#005f5f",
    "vim.leader": "<space>",
    "vim.incsearch": true,
    "vim.useSystemClipboard": true,
    "vim.useCtrlKeys": true, // disable vscode ctrl key
    "vim.hlsearch": true,
    "vim.easymotion": true,
    "vim.timeout": 350,
    "vim.highlightedyank.enable": true,
    "vim.highlightedyank.color": "rgba(245, 40, 145, 0.8)",
    "vim.searchHighlightColor": "rgba(75, 75, 75, 0.8)",
    "vim.history": 200,
    "vim.insertModeKeyBindings": [
        // Quick swap from --INSERT-- to --NORMAL-- 
        {
            "before": [
                "j",
                "j"
            ],
            "after": [
                "<Esc>"
            ]
        },
        {
            "before": [
                "j",
                "k"
            ],
            "after": [
                "<Esc>"
            ]
        }
    ],
    "vim.normalModeKeyBindings": [
        // Go left window
        {
            "before": [
                "<C-h>"
            ],
            "after": [
                "<C-w>",
                "h"
            ]
        },
        // Go right window
        {
            "before": [
                "<C-l>"
            ],
            "after": [
                "<C-w>",
                "l"
            ]
        },
        // Prev tab
        {
            "before": [
                "<C-k>"
            ],
            "commands": [
                ":tabnext"
            ]
        },
        // Next tab
        {
            "before": [
                "<C-j>"
            ],
            "commands": [
                ":tabprev"
            ]
        },
        // Search File
        // {
        //     "before": [
        //         "<leader>",
        //         "f"
        //     ],
        //     "commands": [
        //         "workbench.action.quickOpen"
        //     ]
        // },
        // Search (Grep)
        // {
        //     "before": [
        //         "<leader>",
        //         "F"
        //     ],
        //     "commands": [
        //         "workbench.action.findInFiles"
        //     ]
        // },
        // Hide search highlight
        {
            "before": [
                "<leader>",
                "h"
            ],
            "commands": [
                ":nohl"
            ]
        },
        // SAVE File
        {
            "before": [
                "<leader>",
                "w"
            ],
            "commands": [
                "workbench.action.files.saveAll"
            ]
        },
        // Close tab
        {
            "before": [
                "<leader>",
                "c"
            ],
            "commands": [
                ":q"
            ]
        },
        // Format
        {
            "before": [
                "<leader>",
                "l",
                "f"
            ],
            "commands": [
                "editor.action.formatDocument"
            ]
        },
        // Comment line
        {
            "before": [
                "<leader>",
                "/"
            ],
            "commands": [
                "editor.action.commentLine"
            ]
        },
        // Toggle Explorer
        {
            "before": [
                "<leader>",
                "e"
            ],
            "commands": [
                "workbench.action.toggleSidebarVisibility"
            ]
        },
        // Enter Sidebar
        {
            "before": [
                "<leader>",
                "E"
            ],
            "commands": [
                "workbench.view.explorer"
            ]
        },
        // Easymotion - <Leader>s: Find(Search) {char} forward and backward.
        // https://github.com/easymotion/vim-easymotion/blob/master/doc/easymotion.txt#L86
        {
            "before": [
                "<leader>",
                "s"
            ],
            "after": [
                "<leader>",
                "<leader>",
                "s"
            ]
        },
        // Go Next Error or Warning
        {
            "before": [
                "<leader>",
                "p",
                "l"
            ],
            "commands": [
                "editor.action.marker.nextInFiles"
            ]
        },
        // Go Prev Error or Warning
        {
            "before": [
                "<leader>",
                "p",
                "h"
            ],
            "commands": [
                "editor.action.marker.prevInFiles"
            ]
        },
        // Insert Empty line after
        {
            "before": [
                "<leader>",
                "o"
            ],
            "after": [
                "o",
                "<ESC>"
            ]
        },
        // Insert Emprt line before
        {
            "before": [
                "<leader>",
                "O"
            ],
            "after": [
                "O",
                "<ESC>"
            ]
        },
        // Go to References
        {
            "before": [
                "<leader>",
                "r"
            ],
            "commands": [
                "editor.action.goToReferences"
            ]
        },
        // Move Current Tab (Buffer) To Left Window
        {
            "before": [
                "<leader>",
                "b",
                "j"
            ],
            "commands": [
                "workbench.action.moveEditorToPreviousGroup"
            ]
        },
        // Move Current Tab (Buffer) To Right Window
        {
            "before": [
                "<leader>",
                "b",
                "k"
            ],
            "commands": [
                "workbench.action.moveEditorToNextGroup"
            ]
        },
        // Move tab to right (+1 index)
        {
            "before": [
                "<leader>",
                "b",
                "."
            ],
            "commands": [
                ":tabm +1"
            ]
        },
        // Move tab to left (-1 index)
        {
            "before": [
                "<leader>",
                "b",
                ","
            ],
            "commands": [
                ":tabm -1"
            ]
        },
        // Go Back
        {
            "before": [
                "<C-O>",
            ],
            "commands": [
                "workbench.action.navigateBack"
            ]
        },
        // Go Forward
        {
            "before": [
                "<C-I>",
            ],
            "commands": [
                "workbench.action.navigateForward"
            ]
        },
        // Show all symbol in current file
        {
            "before": [
                "<leader>",
                "d"
            ],
            "commands": [
                "workbench.action.gotoSymbol"
            ]
        },
        // Show all symbol in workspace
        {
            "before": [
                "<leader>",
                "D"
            ],
            "commands": [
                "workbench.action.showAllSymbols"
            ]
        },
        // Github Copilot
        {
            "before": [
                "<leader>",
                "p"
            ],
            "commands": [
                "workbench.action.openQuickChat.copilot"
            ]
        },
        // Tele (from nvim), require FindItFaster vscode Extension
        {
            "before": [
                "<leader>",
                "f"
            ],
            "commands": [
                "find-it-faster.findFiles"
            ]
        },
        {
            "before": [
                "<leader>",
                "F",
            ],
            "commands": [
                "find-it-faster.findWithinFiles"
            ]
        },
        {
            "before": [
                "<leader>",
                "z"
            ],
            "commands": [
                "find-it-faster.resumeSearch"
            ]
        },
        // Rust
        {
            "before": [
                "<leader>",
                "l",
                "d"
            ],
            "commands": [
                "rust-analyzer.openDocs"
            ]
        }
    ],
    "vim.visualModeKeyBindings": [
        // Comment multiple line
        {
            "before": [
                "<leader>",
                "/"
            ],
            "commands": [
                "editor.action.commentLine"
            ]
        },
        // Github Copilot
        {
            "before": [
                "<leader>",
                "p"
            ],
            "commands": [
                "workbench.action.openQuickChat.copilot"
            ]
        }
    ],
