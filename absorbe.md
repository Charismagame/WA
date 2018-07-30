function() 
    local absorbAmount = select(16,WA_GetUnitBuff("player",GetSpellInfo(77535)))
    --print(absorbAmount)
    if absorbAmount then 
        absorbAmount = absorbAmount / 1000 
        return string.format("%i%c",absorbAmount,75) 
    else
        return ""
    end 
end 
