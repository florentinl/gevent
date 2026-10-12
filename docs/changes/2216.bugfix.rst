Fixed a semaphore acquired by a native thread raising ``LoopExit`` when
the main thread waits on it with an otherwise idle hub. This also fixes
monkey-patched logging handler locks used by native background threads
during application startup.
