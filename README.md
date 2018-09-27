# seduploader_build_0x20abb3f1
APT 28 prober

#bug
在sub_100022e7这个函数中,对sub_10002393的函数调用, 他的参数错了, 应该是(BYTE*)&a1 + 1, 而不是(BYTE*)&a1 + 3.
这个BUG导致函数名哈希值生成错误, 继而导致无法找到正确的函数地址, 所以这个病毒有部分功能并未成功完成.
