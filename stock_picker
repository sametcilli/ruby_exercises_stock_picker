def stock_picker(arr)
  profits = []
  values = []
  arr.each_index do |key|
    if (key +1)<arr.length
      profits.push(arr[key + 1,(arr.length - (key+1))].max - arr[key])
      values.push([arr[key + 1,(arr.length - (key+1))].max, arr[key]])
    else
      profits.push(0)
      values.push([0, arr[key]])
      values.select! do |val|
         (val[0] - val[1] == profits.max)
      end  
    end
  end
  values
end


p stock_picker([17,3,6,17,3,6,17,3,6,17,3,6,17])
