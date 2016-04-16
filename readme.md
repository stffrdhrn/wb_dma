Clone of wb_dma from http://opencores.org/project,wb_dma

# Wishbone DMA controller

```
module wb_dma_top(clk_i, rst_i,

        /* wishbone side 0 */
	wb0s_data_i, wb0s_data_o, wb0_addr_i, wb0_sel_i, wb0_we_i, wb0_cyc_i,
	wb0_stb_i, wb0_ack_o, wb0_err_o, wb0_rty_o,
	wb0m_data_i, wb0m_data_o, wb0_addr_o, wb0_sel_o, wb0_we_o, wb0_cyc_o,
	wb0_stb_o, wb0_ack_i, wb0_err_i, wb0_rty_i,

        /* wishbone side 1 */
	wb1s_data_i, wb1s_data_o, wb1_addr_i, wb1_sel_i, wb1_we_i, wb1_cyc_i,
	wb1_stb_i, wb1_ack_o, wb1_err_o, wb1_rty_o,
	wb1m_data_i, wb1m_data_o, wb1_addr_o, wb1_sel_o, wb1_we_o, wb1_cyc_o,
	wb1_stb_o, wb1_ack_i, wb1_err_i, wb1_rty_i,

        /* dma interface */
	dma_req_i, dma_ack_o, dma_nd_i, dma_rest_i,

        /* interrupt */
	inta_o, intb_o
	);

```

## Details (from original site)

This is a simple DMA/Bridge IP core. It has two WISHBONE interface. It can perform DMA transfers between the two interfaces or on the same interfaces. 

Some of the main features are: 

- Up to 31 DMA Channels 
- 2, 4 or 8 priority levels 
- Linked List Descriptors support 
- Circular Buffer support 
- FIFO buffer support 
- Software & Hardware handshake support 
- Automatic Channel Registers Reload support 
- Fully configurable 

Please see the spec for more details !
