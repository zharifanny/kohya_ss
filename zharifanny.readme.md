1. Export path to use opt instead of usr : export PATH="/opt/homebrew/bin:$PATH"
2. 
3. Modified The Script  : #  If the requirements are validated, run the kohya_gui.py script with the command-line arguments
                            if python3.10  "$SCRIPT_DIR"/tools/validate_requirements_unix.py -r "$SCRIPT_DIR"/requirements_unix.txt; then
                            python3.10 "$SCRIPT_DIR/kohya_gui.py" "$@"
                            fi

3. Add tk package       : brew install python-tk@3.10
