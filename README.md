# APB_slave
Verilog-based APB Slave design following AMBA APB 2.0 protocol with configurable data/address widths. Includes a watchdog timer that raises PSLVERR if PENABLE isn't asserted within 10 clock cycles. Comes with a testbench to verify read/write and watchdog error behavior.
