// 声明合约使用的许可证为MIT许可证  
// SPDX-License-Identifier: MIT   

// 指定合约编译器版本为0.8.0及以上，但不包括0.9.0    
pragma solidity ^0.8.0;    
  
    // 定义一个名为InsertSort的合约  
contract InsertSort {    
  
    // 插入排序函数，接受一个int类型的数组（长度为5）作为参数  
        // 声明一个公共的、纯函数（不修改区块链状态）的插入排序方法  
    function insertSort(int[5] memory arr) public pure returns (int[5] memory) { 

        // 获取数组的长度，虽然在这里是固定的5，但为了提高代码的可读性仍然声明了一个变量     
        uint n = arr.length;    
  
        // 外层循环，从数组的第二个元素开始遍历到最后一个元素  
        for (uint i = 1; i < n; i++) {   
            // 将当前元素存储在key变量中   
            int key = arr[i];    
            // 初始化内层循环的索引j，为当前元素的前一个位置  
            uint j = i - 1;    
  
            // 内层循环，用于将key插入到已排序部分的正确位置  
                // 当j没有越界且arr[j]大于key时，继续循环  
            while (j >= 0 && arr[j] > key) {  
                // 将arr[j]向右移动一位    
                arr[j + 1] = arr[j];    
                // 将j减1，继续比较前一个元素  
                j = j - 1;    
            }    
            // 将key插入到正确的位置  
            arr[j + 1] = key;    
        }    
        // 返回排序后的数组  
        return arr;    
    }    
  
    // 获取排序后的数组的方法，接受一个int类型的数组（长度为5）作为参数    
        // 声明一个公共的、纯函数（不修改区块链状态）的获取排序后数组的方法  
    function getSortArr(int[5] memory arr) public pure returns (int[5] memory) {   
        // 调用插入排序函数并返回结果  
        // 调用insertSort函数对传入的数组进行排序，并返回排序后的数组  
        return insertSort(arr);    
    }    
}
