.PHONY: build install clean

# Compiles the source files into object files and archives them into a static library
build: personal_helpers.c personal_helpers.h
    gcc -c personal_helpers.c -o personal_helpers.o
    ar -rc libpersonal_helpers.a personal_helpers.o

# Installs the library (this example won't actually run in the GitHub Actions workflow due to permission issues)
install: build
    @echo "Skipping install step in CI environment"

# Cleans up object files and the library file
clean:
    rm -f personal_helpers.o
    rm -f libpersonal_helpers.a
