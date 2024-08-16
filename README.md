This is the same as legacy SPI library, but added two lines of code.

On beginTranscation(), noInterrupts(); is called to avoid interrupt handlers ruining transactions.
On endTransaction(), interrupts(); is called to re-enable interrupts. 