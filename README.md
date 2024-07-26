# lk2nd

A fork from [msm8916-mainline/lk2nd](https://github.com/msm8916-mainline/lk2nd)

## How to build

- lk2nd

	```
	make TOOLCHAIN_PREFIX=arm-none-eabi- lk2nd-msm8953
	```

- lk1st

	```
	make TOOLCHAIN_PREFIX=arm-none-eabi- LK2ND_BUNDLE_DTB="apq8053-lenovo-sparrow.dtb" LK2ND_COMPATIBLE="lenovo,msm8953_64" lk1st-msm8953
	```

	- Sign `emmc_appsboot.mbn` with [qtestsign](https://github.com/msm8916-mainline/qtestsign)

		```
		./qtestsign.py aboot emmc_appsboot.mbn
		```

