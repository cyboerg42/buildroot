output/build/linux-5.8/arch/riscv/boot/dts/kendryte/k210.dts

```
&qspi0 {
    status = "okay";
//  mmc@0 {
/*      compatible = "mmc-spi-slot";
 *      reg = <0>;
 *      spi-max-frequency = <5000000>;
 *      voltage-ranges = <3200 3400>;
 *      disable-wp;
 *      disable-cd;
 *  };
 */
};
```

output/build/linux-5.8/arch/riscv/boot/dts/kendryte/k210.dtsi

```
qspi0: spi@52000000 {
  compatible = "kendryte,k210-spi", "sifive,spi0";
  reg = <0x52000000 0x1000000>;
  interrupt-parent = <&plic0>;
  interrupts = <35>;
  clocks = <&sysctl K210_CLK_CPU>;
  #address-cells = <1>;
  #size-cells = <0>;
  };
```
